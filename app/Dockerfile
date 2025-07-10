# Usamos una imagen más ligera y específica para Python
FROM python:3.9-slim

# Directorio de trabajo
WORKDIR /app

# Instalamos dependencias del sistema (si las hay) y limpiamos caché
RUN apt-get update && apt-get install -y --no-install-recommends \
    && rm -rf /var/lib/apt/lists/*

# Copiamos solo lo necesario (mejora el caching de Docker)
COPY requirements.txt .
COPY app.py .

# Instalamos dependencias de Python
RUN pip install --no-cache-dir -r requirements.txt

# Exponemos el puerto que usa web.py (por defecto: 8080)
EXPOSE 8080

# Comando para ejecutar la app (web.py usa el puerto directamente en el código)
CMD ["python", "app.py"]