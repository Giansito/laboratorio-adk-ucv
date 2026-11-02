# Laboratorio ADK UCV – Mono-agente con Google ADK

Agente académico básico construido con **Google ADK** y **Python**, con dependencias gestionadas por **Poetry**.

El agente responde en español con lenguaje simple y usa la herramienta `explicar_concepto` para explicar conceptos registrados (API, algoritmo, base de datos).

## Requisitos

- Python 3.11 o superior
- Poetry
- API key de Google Gemini ([Google AI Studio](https://aistudio.google.com/apikey))

## Instalación

```bash
poetry install
```

Crear un archivo `.env` en la raíz del proyecto:

```
GOOGLE_GENAI_USE_VERTEXAI=FALSE
GOOGLE_API_KEY="TU_API_KEY"
```

## Ejecución

Modo consola:

```bash
poetry run adk run agente_ucv
```

Interfaz web (abrir http://localhost:8000):

```bash
poetry run adk web --port 8000
```

## Estructura

```
laboratorio-adk-ucv/
├── agente_ucv/
│   ├── __init__.py
│   └── agent.py
├── tests/
│   └── test_agent.py
├── .env
├── pyproject.toml
├── README.md
└── .gitignore
```
