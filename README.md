# Autor: Gerardo Figueroa
# Fecha: 01/05/26
#
# app-langchain1
Objetivo:
Test LangChain utiliza un modelo como agente para analizar datos de un archivo con lenguaje natural

# 🚀 IA Sales Analyzer: LangChain + Groq + Streamlit

Esta aplicación permite realizar consultas en lenguaje natural sobre archivos de ventas en formato CSV. Utiliza el poder de los agentes de **LangChain** y la velocidad de inferencia de **Groq Cloud** para analizar datos sin necesidad de escribir código SQL o Pandas manualmente.

## 🌟 Características

*   **Análisis Multitabla:** Capacidad para seleccionar entre diferentes archivos CSV en el directorio.
*   **Interfaz Amigable:** Construida con Streamlit, incluye visualización previa de los datos.
*   **Procesamiento Inteligente:** Usa el modelo `Llama-3.3-70b` para razonar sobre las columnas y realizar cálculos complejos (sumas, promedios, comparaciones).
*   **Resultados Estructurados:** Respuestas formateadas en tablas de Markdown para una lectura clara.

## 🛠️ Tecnologías Utilizadas

*   **Python 3.10+**
*   **Streamlit:** Para la interfaz de usuario web.
*   **LangChain & LangChain-Experimental:** Para la lógica del agente de datos.
*   **Groq Cloud API:** Como motor de inteligencia artificial (LLM).
*   **Pandas:** Para la manipulación local de datos.

## 📋 Requisitos Previos
Para correrla localmente:
Antes de correr la aplicación, asegúrate de tener una API Key de Groq. Puedes obtenerla gratis en [Groq Cloud Console](https://console.groq.com/).

## 🚀 Instalación y Uso Local

1. **Clonar el repositorio:**
   ```bash
   git clone [https://github.com/tu-usuario/app-langchain1.git](https://github.com/tu-usuario/app-langchain1.git)
   cd app-langchain1
Instalar dependencias:

Bash
pip install -r requirements.txt
Configurar variables de entorno:
Crea un archivo .env o exporta tu clave directamente:

Bash
export GROQ_API_KEY="tu_api_key_aquí"
Ejecutar la aplicación:

Bash
streamlit run app.py
☁️ Despliegue en Streamlit Cloud
Para desplegar esta app en la nube:

Sube este repositorio a tu GitHub.

Conecta tu cuenta de GitHub con Streamlit Cloud.

En la configuración avanzada (Secrets), añade tu clave:

Ini, TOML
GROQ_API_KEY = "gsk_..."
⚠️ Nota sobre Seguridad
Esta aplicación utiliza allow_dangerous_code=True dentro del Agente de Pandas. Esto permite que el LLM ejecute código Python localmente para procesar los datos. Asegúrate de utilizar archivos CSV de fuentes confiables.
