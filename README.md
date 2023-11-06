

## Repositorio del Reporte Técnico 
<summary>

<div align="center">  
<!--![titulo: DESARROLLO DE PROTOTIPO: METODOLOGÍA CON APRENDIZAJE PROFUNDO PARA EL PRONÓSTICO A CORTO PLAZO DE DEMANDA DE ENERGÍA CON DATOS EN ADELANTO]-->
  <img src="https://github.com/yanhmada/Biociencias_2023/blob/dbb966a406a5c67c797517a251a514ca9fc65ef7/Mycorrhiza/title.png"
</div>
</summary>


#### CONVENIO CENACE-UNISON 2023-2025
<br>
Este repositorio contiene las libretas relacionadas al desarrollo de prototipo para la metodología para el pronóstico a corto plazo de consumo de energía eléctrica de la zona del Noroeste de México.
<br>
<br>
Este modelo parte del reporte técnico LSTM Encoder-Decoder para la estimación de demanda de carga de electricidad a corto plazo en el noroeste de México>, Unison-CENACE (15 de agosto de 2022).  <br>
A partir de este modelo base se hace una modificación a su arquitectura con el fin de obtener:<br>
1. Una reducción en términos generales de la métrica de performance MAPE en comparación con lo obtenido con el modelo base, en particular en los días de inestabilidad climática.<br>
2. Capacidad de adaptación mínima para recibir cualquier variable por adelanto, incluyendo las variables meteorológicas. <br>
Cabe destacar que los modelos se entrenaron con datos reales-medidos sin considerar la incertudimbre de las variables de clima. 
<br><br>
En este análisis se manejan 4 variantes del modelo, las cuáles son:
<br>
* a) Sin variables en adelanto.<br>
* b) Sólo la primera componente principal en adelanto. <br>
* c) Las dos componentes principales y los días festivos en adelanto.<br>
* d ) Lo mismo que en c) más el día de la semana en adelanto<br>
<br>
## Contenido:
- **Tratamiento inicial de datos.** Libreta Y00-JNB0_Data_Cleaning_gpo1.ipynb<br>
- **Diseño y entrenamiento del modelo.**Libreta Y00-JNB1 Data processing (training test validation).ipynb y libreta Y00-JNB2 LSTM Encoder-Decoder_model.ipynb. Este par de libretas se ajustan a cada una de las variantes del modelo, por lo que se encuentran en las subcarpetas de cada variante mencionada.<br>
- ** Pronóstico diario** Libreta Y00-JNB3_Daily_Forecasting.ipynb En esta libreta se extraen los datos del modelo para generar el pronóstico del día siguiente.
<br><br>
Análisis de resultados se pueden consultar [aquí](https://2023fmodel.streamlit.app/)

Noviembre ~ 2023

<summary><div align="center">
  <img src="https://github.com/yanhmada/Biociencias_2023/blob/6fea1932a416d32d2df1a5db0691ac795686db06/Mycorrhiza/bottom_cenace.png">
</div>
</summary>
