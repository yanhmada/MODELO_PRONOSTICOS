

## Repositorio del Reporte Técnico 

<div align="center">  
<img src="https://github.com/yanhmada/Biociencias_2023/blob/dbb966a406a5c67c797517a251a514ca9fc65ef7/Mycorrhiza/title.png"
</div>
<div dir="ltr">
## CONVENIO CENACE-UNISON 2023-2025

Este repositorio contiene las libretas relacionadas al desarrollo de prototipo para la metodología para el pronóstico a corto plazo de consumo de energía eléctrica de la zona del Noroeste de México.


Este modelo parte del reporte técnico "LSTM Encoder-Decoder para la estimación de demanda de carga de electricidad a corto plazo en el noroeste de México", Unison-CENACE (15 de agosto de 2022).  
A partir de este modelo base se hace una modificación a su arquitectura con el fin de obtener:

1. Una reducción en términos generales de la métrica de performance MAPE en comparación con lo obtenido con el modelo base, en particular en los días de inestabilidad climática.
2. Capacidad de adaptación mínima para recibir cualquier variable por adelanto, incluyendo las variables meteorológicas.  

En este análisis se manejan 4 variantes del modelo, las cuales son:
* a) Sin variables en adelanto.
* b) Sólo la primera componente principal en adelanto.
* c) Las dos componentes principales y los días festivos en adelanto.
* d) Lo mismo que en c) más el día de la semana en adelanto. <br>

3. Flexibilidad para realizar el pronóstico a las 11:00 AM, 12:00 PM, etc. del día anterior al día a pronosticar, con la posibilidad de actualizar la información con la que se cuente hasta el momento donde se efectúa el pronóstico.
<br>
4. Flexibilidad para incorporar en una versión ulterior con cambios mínimos los datos meteorológicos por hora.

## Contenido:
- **Tratamiento inicial de datos.** Libreta `Y00-JNB0_Data_Cleaning_gpo1.ipynb`
- **Diseño y entrenamiento del modelo.** Libreta `Y00-JNB1 Data processing (training test validation).ipynb` y libreta `Y00-JNB2 LSTM Encoder-Decoder_model.ipynb`. Este par de libretas se ajustan a cada una de las variantes del modelo, por lo que se encuentran en las subcarpetas de cada variante mencionada.
- **Pronóstico diario.** Libreta `Y00-JNB3_Daily_Forecasting.ipynb`. En esta libreta se extraen los datos del modelo para generar el pronóstico del día siguiente.

Análisis de resultados de las 4 variantes del modelo se pueden consultar [aquí](https://2023fmodel.streamlit.app/).

Noviembre ~ 2023
</div>
<div align="center">
  <img src="https://github.com/yanhmada/Biociencias_2023/blob/6fea1932a416d32d2df1a5db0691ac795686db06/Mycorrhiza/bottom_cenace.png">
</div>
