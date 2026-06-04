# Analisis de Resultados de Prueba A/B

El objetivo de este proyecto fue analizar los resultados de una prueba A/B realizada por una tienda online anonima. Se nos proporcionaros los datos de los resultados generados por las pruebas y nuestra tarea fue verificar la validez y confiabilidad de los datos, un analisis exploratorio de los resultados obtenidos por ambos grupos (A y B) y finalmente la aplicacion de pruebas de significancia estadistica para determinar con mayor rigor las diferencia entre los grupos experimentales.

## Habilidades Tecnológicas Utilizadas

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-%230C55A5.svg?style=for-the-badge&logo=scipy&logoColor=%white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75.svg?style=for-the-badge&logo=Plotly&logoColor=white)
![Markdown](https://img.shields.io/badge/markdown-%23000000.svg?style=for-the-badge&logo=markdown&logoColor=white)
![Postgresql](https://img.shields.io/badge/PostgreSQL-4169E1.svg?style=for-the-badge&logo=PostgreSQL&logoColor=white)
![Power Bi](https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Microsoft Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Google Sheets](https://img.shields.io/badge/Google%20Sheets-%2334A853?style=for-the-badge&logo=googlesheets&logoColor=white)
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)


## Preguntas clave

- ¿Cual fue el ingreso de cada grupo por separado?
- ¿Como fueron el volumen de pedidos por grupo?
- ¿Cual fue la diferencia relativa entre los pedidos promedio de cada grupo?
- ¿Cual fue la tasa de conversion diaria por grupo?


## ¿Cual fue el ingreso de cada grupo por separado?

La grafica muestra como los ingresos de ambos grupos fueron muy similares los primeros 5 dias. Posteriormente los ingresos acumulados del grupo B se incrementaron un poco mas que el grupo A y a partir del dia 13 los ingresos del grupo B fueron claramente superiores que los del grupo A. Al final, los ingresos del grupo A fueron: 64554.9, mientras que los ingresos del grupo B fueron: 92840.6. Esto es (64554.9 / 92840.6) x 100 = 69.53 %, es decir que el grupo B tuvo un poco mas de 30% mas de ingresos que el grupo A.

<img width="1179" height="582" alt="Screenshot_20260604142226" src="https://github.com/user-attachments/assets/91bce844-93d7-4d6f-9ed4-e58bddc0db16" />


## ¿Como fueron el volumen de pedidos por grupo?

La grafica muestra un comportamiento interesante respecto al tamaño de pedidos promedio acumulados a lo largo del experimento. 

- Grupo A: El grupo A comenzo arriba del grupo B, pero durante los primeros dias fue a la baja, para posteriormente comenzar a tener un repunte y superar durante algunos dias al grupo B. Despues de lo cual descendio un poco para mantener cierta estabilidad el resto de los dias del experimento.
- Grupo B: El grupo B comenzo abajo del grupo A, pero los primeros dias su comportamiento fue hacia arriba superando por 9 dias al grupo A: Luego el grupo A logro superar al grupo B durante unos dias, mientras que el grupo B se mantuvo con cierta estabilidad. El dia 19 el grupo B tuvo un brusco repunte, superando por mucho al grupo A que se mantuvo estable el resto del experimento. El grupo B mantuvo esa ventaja con cierta estabilidad el resto de los dias.
- Nuevamente los resultados del Test A/B son favorables para el grupo B.

<img width="1181" height="588" alt="Screenshot_20260604142431" src="https://github.com/user-attachments/assets/ead7660e-a183-43aa-88d2-0e383c3bbc02" />


## ¿Cual fue la diferencia relativa entre los pedidos promedio de cada grupo?

La grafica anterior nos permite ver con exactitud cual fue la diferencia porcentual dia con dia del grupo B con respecto al grupo A en lo referente al tamaño de pedido promedio acumulado. En realidad hay dos periodos durante los cuales el grupo A fue superior al grupo B, al inicio y en un periodo intermedio. El punto inicial fue el punto mas bajo del grupo B, donde tuvo una diferencia relativa negativa de -21.4% y luego en un punto intermedio con -18.3%. Sin embargo la diferencia relativa mas notable fue cuando el grupo B supero al grupo A por un 41.4%. Al final el grupo B logro una diferencia porcentual relativa positiva del 23.8% con respecto al grupo A.

<img width="1176" height="582" alt="Screenshot_20260604142605" src="https://github.com/user-attachments/assets/513fefac-1784-490e-b383-a6feb4603943" />


## ¿Cual fue la tasa de conversion diaria por grupo?

Debemos observar como la tasa de conversion entre ambos grupos se mantiene en un rango de entre poco mas de 1% hasta poco mas de 6%. El punto mas alto en la tasa de conversion lo tuvo el grupo B con un 6.23%, sin embargo tambien obtuvo el punto de conversion mas bajo con un 1.22%.

La tasa de conversion promedio del grupo B fue ligeramente superior que la del grupo A. No podriamos asumir con seguridad si esta diferencia es realmente significativa, aun con los resultados positivos de los analisis anteriores para el grupo B.

<img width="1266" height="539" alt="Screenshot_20260604142721" src="https://github.com/user-attachments/assets/07d44747-48f8-4337-bff6-4f65effc01ac" />


## Resultados de las pruebas de hipotesis estadisticas

Realizamos la prueba T Student y la prueba Mann-Whitney. En ambos casos el resultado fue que no hay diferencias significativas en el tamaño promedio de compra de los grupos A y B. En la prueba anterior, donde no habiamos filtrado los valores extremos, el resultado era similar. Entonces, segun los resultados de las pruebas, no hay una diferencia significativa entre los grupos A y B.

<img width="1341" height="807" alt="Screenshot_20260604143111" src="https://github.com/user-attachments/assets/ad621e90-1c79-42f9-a6d8-9807aae257fb" />


## Conclusiones y recomendaciones

La recomendacion para este caso segun los analisis realizados, los resultados de las pruebas y la evidencia recogida es que deberiamos detener la prueba y concluir que no hay diferencia entre los grupos. La diferencias observadas en los grupos se debio principalmente a los valores extremos encontrados en el grupo B, que provocaron que los resultados de varios analisis fueran favorables para este grupo. Al eliminar estos valores atipicos pudimos observar que no hay una diferencia notable entre los grupos.

* Recomendacion: Detener la prueba y concluir que no hay diferencias significativas entre los grupos A y B.
