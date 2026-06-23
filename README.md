# 📊 Sales Diagnosis & Churn Analysis: El "Efecto Espejismo" en Europa

<br clear="right"/>
<br/>

> **"¡Las ventas han bajado!"** Tras un 2021 de récords históricos, el negocio empezó a contraerse. Este análisis fue diseñado para responder una pregunta crítica de negocio: **¿Por qué estamos perdiendo ingresos si nuestro ticket medio parece estable?**

<br clear="right"/>
<br/>

<img src="https://github.com/Elian-digital/PowerBI_Sales-Diagnosis-Churn-Analysis/blob/main/images/01_Evolucion_pedidos_ventas.png?raw=true" align="right" width="400" Clasp="image">

A través de este proyecto de Business Intelligence, identifiqué una **caída real del 4% en la facturación global**, ocultada por anomalías métricas, y aislé la verdadera causa raíz: un problema de **fuga masiva de clientes (Churn)** concentrado en un único mercado estratégico.

[📥 Descargar Presentación Ejecutiva en PDF (DataStory ventas.pdf)](./DataStory%20%20ventas.pdf)

<br clear="right"/>



## 🔍 El Proceso de Diagnóstico: Descartando "Sospechosos"

Para resolver la caída de ingresos, el análisis avanzó descartando hipótesis mediante los datos, reduciendo la fricción cognitiva para la toma de decisiones corporativas:

### ❌ Hipótesis 1: ¿Es un problema del catálogo o modas de producto?

<img src="https://github.com/Elian-digital/PowerBI_Sales-Diagnosis-Churn-Analysis/blob/main/images/02_Evolucion_ventas_producto.png?raw=true" align="right" width="400">

* **Diagnóstico:** Se analizó la evolución anual de ventas por producto (*Skywalker, Karstark, The Duel, Stannis, Direwolf*).
* **Conclusión:** El catálogo basado en merchandising de franquicias se mantuvo completamente estable. No había pérdida de interés ni fatiga comercial de producto.

<br clear="right"/>

### ❌ Hipótesis 2: ¿Es un descenso generalizado en los mercados?

<img src="https://github.com/Elian-digital/PowerBI_Sales-Diagnosis-Churn-Analysis/blob/main/images/03_Evolucion_ventas_pais.png?raw=true" align="right" width="400">

* **Diagnóstico:** Segmentación geográfica del comportamiento de facturación del Top 5 de países (*Sweden, Netherlands, Italy, United Kingdom, Germany*).
* **Conclusión:** Casi todos los mercados muestran una notable estabilidad a lo largo del tiempo... **excepto uno**.

<br clear="right"/>

### 🚨 La Causa Raíz: ¿Qué ocurrió en Alemania?

<img src="https://github.com/Elian-digital/PowerBI_Sales-Diagnosis-Churn-Analysis/blob/main/images/04_Evolucion_ventas_Alemania.png?raw=true" align="right" width="400">

Alemania experimentó un crecimiento explosivo en 2020, pero en 2023 sufrió un desplome drástico en su facturación que terminó desestabilizando la foto global y empujando los KPI de la compañía a la baja. Ese patrón de caída libre no se repite en ningún otro país de la red.

<br clear="right"/>



## 💡 El "Efecto Espejismo" de AC Fermentum

Al perforar en los datos de Alemania mediante técnicas de *Drill-Down*, descubrimos que el comportamiento macro del país estaba completamente monopolizado por un único cliente/distribuidor: **AC Fermentum**.

### 1. La distorsión del Ticket Medio

<img src="https://github.com/Elian-digital/PowerBI_Sales-Diagnosis-Churn-Analysis/blob/main/images/05_Ticket_medio_alemania_mundo.png?raw=true" align="right" width="400">

En 2022, el ticket medio global de la compañía parecía subir con fuerza, dando a la junta directiva una falsa sensación de crecimiento y salud financiera. En realidad, era **AC Fermentum** la que distorsionaba la foto al inflar temporalmente la media global debido a un aumento puntual de su ticket medio. 

<br clear="right"/>
<br/>

<img src="https://github.com/Elian-digital/PowerBI_Sales-Diagnosis-Churn-Analysis/blob/main/images/06_Ingresos_empresas_alemania.png?raw=true" align="right" width="400">

La historia cobró un sentido analítico absoluto al aislar los ingresos de las empresas en Alemania: si el país se movía de forma tan volátil, era porque esta cuenta estaba arrastrando al mercado entero.

<br clear="right"/>

<br clear="right"/>

### 2. El Declive y el Churn Real

<img src="https://github.com/Elian-digital/PowerBI_Sales-Diagnosis-Churn-Analysis/blob/main/images/08_Paises_Ac_fermentum.png?raw=true" align="right" width="400">

Cuando el ticket promedio de AC Fermentum tocó su punto más alto en 2022, comenzó el declive real del volumen de negocio. El modelo analítico destapó que el "boom" de esta distribuidora venía impulsado por bloques de clientes de **Italia, Polonia, Portugal y el Reino Unido**. 

En 2023, estos bloques de compradores internacionales **desaparecieron por completo del gráfico de AC Fermentum**. Dejaron de comprarles de golpe. Estamos ante un escenario de **Churn real**: clientes finales que se fugaron de nuestra red comercial.

<br clear="right"/>

---

## 🛠️ Arquitectura Técnica y Respaldo del Dato

Para construir esta narrativa de negocio y asegurar que los insights fueran 100% confiables para la toma de decisiones, se desarrolló un backend robusto en Power BI que soporta la integridad de este reporte:

* **ETL Avanzado (Power Query):** Extracción, limpieza, normalización y transformación de la estructura de ventas fragmentada de los comercios online europeos para corregir anomalías estructurales de origen.
* **Modelado de Datos Avanzado:** Diseño e implementación de un modelo en estrella (*Star Schema*) óptimo para garantizar un alto rendimiento en el procesamiento de millones de registros y asegurar la escalabilidad del informe.
* **Cálculos DAX Complejos:** Desarrollo de métricas e indicadores dinámicos para calcular con precisión las tasas de retención, la identificación temporal del Churn de clientes (*fuga activa*) y el ticket promedio real ponderado entre los años 2018 y 2024.



## 📋 Conclusiones y Próximos Pasos (Acción de Negocio)

El dataset actual ha permitido diagnosticar con precisión el *dónde*, el *cuándo* y el *cuánto* del impacto financiero. Sin embargo, para resolver las causas operativas de por qué se marcharon estos bloques de clientes, se propone a la dirección abrir tres líneas de investigación:

1. **H1 (Aparición de Competencia):** Auditar si nuevos proveedores en los mercados de Polonia, Italia o Portugal captaron a los compradores clave que antes dependían de nuestra red de distribución in Alemania.
2. **H2 (Problemas Operativos Internos):** Cruzar este histórico con datos de operaciones para revisar si existieron retrasos críticos en logística, roturas de stock o cambios contractuales bruscos en el periodo 2022-2023.
3. **H3 (Contexto Macroeconómico):** Evaluar el impacto de la inflación y las regulaciones aduaneras post-periodo en países clave que pudieran haber reducido la demanda de importación de merchandising.

---

## 📬 Contacto y Redes

Si quieres conocer el detalle técnico del modelo DAX, auditar el proceso de ETL o discutir cómo la visualización de datos puede resolver problemas complejos de negocio, no dudes en contactarme:

* **LinkedIn:** [in/eliandaghoum](https://linkedin.com/in/eliandaghoum)
* **Email:** [eliandaghoum@gmail.com](mailto:eliandaghoum@gmail.com)
* **GitHub:** [@Elian-digital](https://github.com/Elian-digital)
