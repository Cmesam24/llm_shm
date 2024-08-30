Repositorio de prueba para implemenry LLM y una aplicacion web 
# 1. Instalacion de ollama 

Para instalar ollama accedemos a la pagina de https://ollama.com/download/linux
Ejecutamos el siguiente codigo para instalar

``````
curl -fsSL https://ollama.com/install.sh | sh

´´´´´´

# 2. Ejecutar el servidor 

Una vez instalado se ejecuta el servidor ollama con el siguiente comando 
````
$ ollama serve
````
# 3. Descargar algun modelo 

En la pagina de modelos de ollama se busca el modelo deseado y se decarga con el siguiente comando 
````
$ ollama pull tinyllama
````
# 3. Peticion API  
Para realizar una petición basica a la API de ollama se sigue la siguiente estructura 

``````
curl http://localhost:11434/api/generate -d '{
  "model": "llama3",
  "prompt": "Why is the sky blue?"
}'

``````



