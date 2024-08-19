import openai 
openai.api_key = “XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX”
def obtener_datos_usuario():
profesion = input("¿Qué tipo de profesional de la salud estás buscando? (por ejemplo, psicóloga, psicopedagoga, fonoaudióloga, terapista ocupacional) ")
experiencia = input("¿Qué tipo de experiencia es relevante para el puesto? (por ejemplo, experiencia en autismo) ")
   	 if profesion.lower() == 'esc':
       		 return None, None
    	return profesion, experiencia


def crear_prompt_descripcion(profesion, experiencia):
prompt = (
f"Generar una descripción de empleo para un puesto de {profesion} en un consultorio médico. "
        		f"El profesional debe tener {experiencia}. "
f"La descripción debe ser atractiva, inclusiva y detallada, destacando la importancia de la especialización "
f"en terapia cognitiva conductual. También se deben mencionar los beneficios del puesto y el impacto positivo "
       		f"en la vida de los niños con autismo y sus familias."
    	)
    	return prompt


def generar_descripcion(prompt):
   	try:
              		response = openai.ChatCompletion.create(
            			model="gpt-3.5-turbo",
            			messages=[
{"role": "system", "content": "System message introducing the chat"},
                			{"role": "user", "content": prompt}
           			 ],
            			max_tokens=250
       		 )
       		 return response['choices'][0]['message']['content']
    	except openai.error.OpenAIError as e:
        		print("Error al generar la descripción:", e)
        		return None


while True:
   	 # Paso 1: Obtener datos del usuario
    	profesion, experiencia = obtener_datos_usuario()
   	 if profesion is None:
       		 print("Saliendo del programa...")
        		break
    	# Paso 2: Crear el prompt para la descripción de empleo
    	prompt_descripcion = crear_prompt_descripcion(profesion, experiencia)
    	print("Prompt creado para la descripción de empleo:", prompt_descripcion)
    	# Paso 3: Generar la descripción de empleo
    	descripcion_empleo = generar_descripcion(prompt_descripcion)
    	if descripcion_empleo:
        		print("Descripción de empleo generada:")
        		print(descripcion_empleo)
