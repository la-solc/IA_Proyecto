# IA_Proyecto
Proyecto para el curso de Inteligencia Artificial para las Ciencias e Ingeniería correspondiente al semestre 2023-2. 
Proyecto realizado por:

Marisol Correa Gutiérrez (Bioingeniería)
C.C. 1007223653

Manuela Ospina Giraldo (Bioingeniería)
C.C.  1007232820

Eliana Salas Villa (Bioingeniería)
C.C. 1193579584


Competencia: H1N1 and Seasonal Flu Vaccines - Aprendizaje para predecir un problema multi-etiqueta con las vacunas contra la gripe H1N1 y estacional

Para agregar un conjunto de datos de Kaggle a Google Colab utilizando un archivo JSON de token de Kaggle, siguiendo estos pasos:

1. Preparar el token de Kaggle:
   - Ir al perfil en Kaggle (https://www.kaggle.com/account).
   - En la sección "API", hacer clic en "Create New API Token". Esto descargará un archivo JSON llamado kaggle.json a tu computadora. Este archivo contiene tus credenciales de Kaggle.

2. Subir el archivo JSON a Google Colab:

   - Abrir Google Colab (https://colab.research.google.com/).
   - En Colab, hacer clic en el ícono de carpeta en el panel izquierdo para abrir la sección de archivos.
   - Hacer clic en el ícono de "Subir" y selecciona el archivo kaggle.json descargado previamente. Esto subirá el archivo al entorno de Colab.

3. Instalar la biblioteca de Kaggle:

   - Ejecutar el siguiente comando en una celda de Colab para instalar la biblioteca de Kaggle:
     
```
     !pip install kaggle
```
     

4. Mover el archivo JSON a la ubicación correcta:

   - Mover el archivo kaggle.json al directorio correcto donde la biblioteca de Kaggle espera encontrarlo. Utilizar el siguiente comando:

     ```
     !mkdir -p ~/.kaggle
     !mv kaggle.json ~/.kaggle/
     ```
     

5. Cambiar los permisos del archivo JSON:

   Para proteger tus credenciales, se debe asegurar que el archivo JSON tenga permisos adecuados. Para ello, se utiliza el siguiente comando para establecer permisos restrictivos:

     ```
     !chmod 600 ~/.kaggle/kaggle.json
     ```
     

7. Descargue el conjunto de datos de Kaggle:

   - Usar la biblioteca de Kaggle para descargar el conjunto de datos que deseas en Colab. 

     ```
     !kaggle datasets download -d <H1N1_Flu_Vaccines>
     ```

   - Esto descarga el conjunto de datos en formato ZIP a el entorno de Colab.

8. Descomprimir el conjunto de datos:

   - Descomprima el archivo ZIP descargado usando el siguiente comando :

     ```
     !unzip <H1N1_Flu_Vaccines.zip>
     ```
     
   - Esto descomprime el conjunto de datos y se puede acceder a los archivos para su análisis.



ENTREGA #2

## Notebook:
[Proyecto_IA](https://colab.research.google.com/drive/1s77dTCO_lwHxf8CKk4WMUZE2s5PxLVh9?usp=sharing)

ENTREGA FINAL

## Notebooks:
[01 - modelos supervisados](https://colab.research.google.com/drive/1bj4SZnySrO_dFzbc_xvIA3PVs7q2LSZp?authuser=1)
[02 - modelos compuestos](https://colab.research.google.com/drive/1y3qbQ_zskMVxRi4y5BwVCwZCjgN_8rzY?authuser=1)
[03 - Variacion de estructuras](https://colab.research.google.com/drive/1s77dTCO_lwHxf8CKk4WMUZE2s5PxLVh9?authuser=1)
[04 - modelos supervisados con datos balanceados](https://colab.research.google.com/drive/1p7Uw27U8gtHg2Do9h4dnKEfFaRTA-ZNi?authuser=1)


## Videos:
[Video entrega 2](https://www.youtube.com/watch?v=8sZhMG-_CPo)

[Video entrega final](https://youtu.be/Dvz3B8Ftvgw)
****
