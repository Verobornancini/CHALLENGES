# Cargo la imágen que voy a utilizar
FROM python:3

# Llamo a mi script de python
ADD Challenge_DeepVision_2019.py /

# Instalo las dependencias necesarias 
RUN pip install numpy
RUN pip install matplotlib
RUN pip install pillow
RUN pip install NMS

# Llevo todos los archivos al directorio de trabajo
COPY . .

# Declaro el puerto por donde se comunica mi contenedor
EXPOSE 1215

# Defino que ejecuto: Ejecución del script n la línea de comando cuando la imagen este cargada
CMD [ "python", "Challenge_DeepVision_2019.py" ]
