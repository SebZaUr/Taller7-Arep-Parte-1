# Lab 7 - Part 1 - Simple LLM

---

## Proyect's Description

 we'll show you how to build a simple LLM application with LangChain. This application will translate text from English into another language. This is a relatively simple LLM application - it's just a single LLM call plus some prompting. Still, this is a great way to get started with LangChain - a lot of features can be built with just some prompting and an LLM call!

After reading this tutorial, you'll have a high level overview of:

- Using language models.
- Using PromptTemplates and OutputParsers.
- Using LangChain Expression Language (LCEL) to chain components together.
- Debugging and tracing your application using LangSmith.
- Deploying your application with LangServe.

---

## Solution Arquitecture

The solution is based on configurable "chains" of modules that make it easy to integrate language models with other tools. These modules are linked to structure complex workflows in applications like chatbots, data assistants, or recommendation systems. LangChain allows combining LLMs with memory storage, document search, and agents to improve the model’s accuracy and adaptability across various tasks, adjusting the solution to specific user needs.

---

## System's componets

- ___Server:___ In this we create a simple FastAPI serve that leverages LangChain's LLM tools to build an API for translation.
- ___Client:___ Make a simple request to us server.

---

## Run Proyect

### Minimum Requirements

- ___Python Version:___ 3.8 or higher
- ___Dependencies:___
  - `fastapi`
  - `uvicorn`
  - `langchain-core`
  - `langchain-openai`
  - `langserve`

## Installation Instructions

1. ___Clone following repository___

    ```bash
    git clone https://github.com/SebZaUr/Taller7-Arep-Parte-1.git
    ```

2. ___Enter the project directory___

    ```bash
    cd Taller7-Arep-Parte-1
    ```

3. ___Create a virtual environment___ (optional, but recommended):

   ```bash
   python3 -m venv langchain_env
   source langchain_env/bin/activate
   ```

4. ___Install all dependencies___

    ```bash
    pip install fastapi uvicorn langchain-core langchain-openai langserve
    ```

5. ___In a terminal run the server___

    ```bash
    python server.py
    ```

6. ___In another terminal run th client___

    ```bash
    python client.py
    ```

---

## Sreenshots Test

![servidor](/LargeChaingServer/img/server.png)
![cliente](/LargeChaingServer/img/client.png)

---

## Licencia

Este proyecto está bajo la licencia de Creative Commons Reconocimiento-CompartirIgual 4.0 Internacional (CC BY-SA 4.0) - Ver el archivo [LICENSE](LICENSE.md) para más detalles.

---

## Autor

- __Sebastian Zamora Urrego__
