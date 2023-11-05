
### CONVENIO CENACE-UNISON 2023-2025
## Desarrollo de prototipo: metodología con aprendizaje profundo para el pronóstico a corto plazo de demanda de energía con datos en adelanto.


<br>
Este repositorio contiene las libretas relacionadas al desarrollo de prototipo para la metodología para el pronóstico a corto plazo de consumo de energía eléctrica de la zona del Noroeste de México.

En este análisis se manejan 4 variantes del modelo, las cuáles son:
a) Sin variables en adelanto.
b) Sólo la primera componente principal en adelanto.
c) Las dos componentes principales y los días festivos en adelanto.
d ) Lo mismo que en c) más el día de la semana en adelanto
<br>
## Contenido:
- ** Tratamiento inicial de datos.** Libreta Y00-JNB0_Data_Cleaning_gpo1.ipynb
- ** Diseño y entrenamiento del modelo.** Libreta Y00-JNB1 Data processing (training test validation).ipynb y libreta Y00-JNB2 LSTM Encoder-Decoder_model.ipynb. Este par de libretas se ajustan a cada una de las variantes del modelo, por lo que se encuentran en las subcarpetas de cada variante.
- ** Pronóstico diario** Libreta Y00-JNB3_Daily_Forecasting.ipynb En esta libreta se extraen los datos del modelo para generar el pronóstico del día siguiente.

Noviembre ~ 2023

<div align="center">
  <img src="https://github.com/yanhmada/Biociencias_2023/blob/6fea1932a416d32d2df1a5db0691ac795686db06/Mycorrhiza/bottom_cenace.png">
</div>
</summary>
