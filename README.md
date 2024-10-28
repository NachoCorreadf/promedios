# Promedios
## Calcular promedio

1 - Importar las librerías necesarias.

2 - Crear un DataFrame (o cargar uno existente).

3 - Calcular el promedio de la columna deseada.

4 - Visualizarlo usando Seaborn.
## Codigo
 ~~~~
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt


data = {
    'Nombre': ['Nacho', 'Agus', 'Luca', 'Lauti', 'Juan'],
    'Edades': [10, 20, 30, 40, 50]
}
df = pd.DataFrame(data)


promedio = df['Edades'].mean()
print(f'El promedio de la columna "Edades" es: {promedio}')


sns.barplot(x='Nombre', y='Edades', data=df)
plt.axhline(y=promedio, color='r', linestyle='--', label='Promedio')
plt.legend()
plt.title('Edades con Promedio')
plt.show()
~~~~
### Por lo tanto, el promedio de la columna "Edades" es 30.

![image](https://github.com/user-attachments/assets/ed43d69f-439c-4c1f-a018-f0330042d2df)
