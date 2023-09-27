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

Para obtener los datos y hacerlos disponibles en el Notebook de Colab, sigue los siguientes pasos:

Paso 1: Instala la API de Kaggle 
```
pip install kaggle
```

Paso 2: Configura las credenciales de Kaggle
```
from kaggle.api.kaggle_api_extended import KaggleApi
```

Paso 3: Especificar la ubicación del archivo JSON de Kaggle. La ruta del archivo .json dependerá de la ubicación en la computadora. Se puede obtener el archivo .json siguiendo la ruta kaggle - perfil - cuenta - tokens de API.
```
api = KaggleApi()
api.authenticate(api_key='ruta/kaggle.json')
```

Paso 4: Descarga el conjunto de datos de Kaggle
Utilizar el comando 'dataset_download_files' con el nombre del conjunto de datos en Kaggle.
```
api.dataset_download_files('arashnic/flu-data', path='.', unzip=True)
```

Paso 5: Carga el conjunto de datos en el Notebook
```
import pandas as pd
df = pd.read_csv('H1N1_Flu_Vaccines.csv')
```

