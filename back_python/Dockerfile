# Usa una imagen base de Python
FROM python:3.9

# Establece el directorio de trabajo en el contenedor
WORKDIR /app

# Copia el archivo de requerimientos y lo instala
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copia el código de la aplicación al contenedor
COPY . .

# Expone el puerto en el que correrá Flask
EXPOSE 5000

# Comando para iniciar la aplicación
CMD ["python", "app.py"]
