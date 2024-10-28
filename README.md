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
    'Valores': [10, 20, 30, 40, 50]
}
df = pd.DataFrame(data)


promedio = df['Valores'].mean()
print(f'El promedio de la columna "Valores" es: {promedio}')


sns.barplot(x='Nombre', y='Valores', data=df)
plt.axhline(y=promedio, color='r', linestyle='--', label='Promedio')
plt.legend()
plt.title('Valores con Promedio')
plt.show()
~~~~
### Por lo tanto, el promedio de la columna "Valores" es 30.

![image](https://github.com/user-attachments/assets/ed43d69f-439c-4c1f-a018-f0330042d2df)
