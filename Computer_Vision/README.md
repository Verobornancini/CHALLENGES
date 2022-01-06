# Challenge---Machine-Learning-Computer-Vision

# El ambiente necesario para correr el archivo Challenge.py posee las siguientes librerias:
# * NMS
# * json
# * matplotlib.pyplot
# * matplotlib.patches
# * Image from PIL

# **PIPELINE**
# El desarrollo del mismo consiste en:
# Obtener un array numpy de bounding boxes(bb)
# Dibujar los bounding boxes sobre la imagen
# Implementar del algoritmo greedy (estándar) de NMS
# Obtener el IOU (Intersection over Union)
# Realizar un test con una imagen de prueba

# ¿Cuál es la ventaja de soft-nms sobre NMS estándar?

# NMS:
# -Selecciona el bounding box con mayor score (M) y suprime los bounding box cuya sobreposicion con el M sea significativa. Para ello genera una lista de bounding boxes (bb) a partir de los cuales elije uno, teniendo en cuenta el score de los mismos.

# Soft-NMS:
# -Por su parte no elimina ningun objeto ya que toma los scores de deteccion de los objetos superpuestos con M, como funciones continuas. De todos modos su confianza es menor. -Es de facil implementación. -Es muy sencillo de integrarlo a cualquier pipeline de deteccion de objetos.
