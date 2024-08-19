IA para Optimización del Reclutamiento de Terapeutas Especializados en Autismo
Descripción del Proyecto
Este proyecto utiliza inteligencia artificial, específicamente modelos de OpenAI como ChatGPT y DALL-E, para generar descripciones de empleo y contenido visual que mejoren el proceso de reclutamiento de terapeutas especializados en autismo. A través de técnicas de Fast Prompting, se optimiza la generación de contenido atractivo y relevante para diferentes roles profesionales en el ámbito de la salud infantil.

Estructura del Proyecto
Generar_Descripciones.ipynb: Cuaderno principal que contiene el código para generar descripciones de empleo y las imágenes relacionadas.
Imágenes Generadas: Carpeta que contiene las imágenes generadas con DALL-E.
descripciones_empleo.csv: Archivo que almacena las descripciones generadas en formato CSV.
Requisitos
Clonar el repositorio:

bash
Copiar código
git clone https://github.com/sastremax/IA-generacion-de-prompts.git
Instalar las dependencias necesarias:

bash
Copiar código
pip install openai pandas jupyterlab
Obtener tu clave de API de OpenAI e insertarla en el código:

python
Copiar código
openai.api_key = "TU_API_KEY"
Instrucciones de Uso
Abre el archivo Generar_Descripciones.ipynb en Jupyter Notebook o JupyterLab.
Sigue las instrucciones en el cuaderno para generar las descripciones de empleo.
Visualiza las imágenes generadas y guarda las descripciones en formato CSV.
Tecnologías Utilizadas
OpenAI API: Modelos ChatGPT y DALL-E.
Pandas: Manejo de datos en formato CSV.
Jupyter Notebook: Plataforma utilizada para ejecutar y probar el código.
Python: Lenguaje principal del proyecto.
Resultados Esperados
Descripciones de empleo bien redactadas, personalizadas para cada tipo de profesional.
Imágenes visualmente atractivas generadas con DALL-E que acompañan las descripciones de empleo.
Aumento en la efectividad del proceso de reclutamiento para terapeutas especializados en autismo.
