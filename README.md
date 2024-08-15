# IA para Optimización del Reclutamiento de Terapeutas Especializados en Autismo

## Descripción del Proyecto
Este proyecto utiliza modelos de inteligencia artificial, como ChatGPT y DALL-E, para generar descripciones de empleo y contenido visual que mejoren el proceso de reclutamiento de terapeutas especializados en autismo. A través de técnicas de Fast Prompting, el proyecto optimiza el uso de recursos para crear contenido atractivo y específico para diferentes puestos profesionales en el ámbito de la salud infantil.

## Estructura del Proyecto
- **`Generar_Descripciones.ipynb`**: Notebook principal que contiene el código para generar descripciones de empleo y las imágenes relacionadas.
- **Imágenes Generadas**: Carpeta que contiene las imágenes generadas con DALL-E.
- **`descripciones_empleo.csv`**: Archivo que almacena las descripciones generadas en formato CSV.

## Instrucciones para Ejecutar el Proyecto
1. Clona el repositorio:
   ```bash
   git clone https://github.com/sastremax/IA-generacion-de-prompts.git

2. Instala las dependencias necesarias:

Asegúrate de tener openai, pandas, y jupyterlab instalados en tu entorno.
bash
Copiar código
pip install openai pandas jupyterlab
Obtén tu clave de la API de OpenAI e insértala en el código:

Puedes obtener tu clave en OpenAI.
3. Inserta tu clave en el notebook en la línea correspondiente:
python
Copiar código
openai.api_key = "TU_API_KEY"
Abre el notebook Generar_Descripciones.ipynb en Jupyter Notebook o JupyterLab y sigue las instrucciones paso a paso para generar las descripciones y las imágenes.
