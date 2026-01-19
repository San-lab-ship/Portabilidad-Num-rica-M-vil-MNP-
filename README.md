# 📱 Portabilidad Numérica Móvil (MNP) (TelcoA-D)

## 🎯 Objetivo
Desarrollar una solución integral basada en Inteligencia Artificial y Ciencia de Datos para automatizar, predecir y optimizar el proceso de portabilidad numérica entre los operadores TelcoA, TelcoB, TelcoC y TelcoD, reduciendo los tiempos de ejecución y minimizando los rechazos operativos.

## 🛑 Descripción del Problema
En el sector de telecomunicaciones, la portabilidad numérica suele enfrentar dos grandes cuellos de botella:
* **Rechazos por Incumplimiento**: Muchas solicitudes se inician sin validar previamente deudas o scoring crediticio, generando costos operativos innecesarios.
* **Errores en el Flujo Operativo**: Documentos ilegibles o caídas de sistemas externos (API) detienen el proceso durante horas o días, afectando la experiencia del cliente (SLA).

## 🏗️ Arquitectura del Sistema
El sistema implementa una arquitectura de servicios desacoplados:
* **MNP Core Gateway**: Motor lógico que gestiona el estado del trámite.
* **Predictive Engine**: Modelo de Machine Learning que evalúa la viabilidad del cliente.
* **Early Warning System (EWS)**: Módulo de alertas automáticas para la recuperación de trámites fallidos.
* **Central DB**: Base de datos relacional simulada que centraliza los movimientos de los 4 operadores.

## 📊 Metodología
Se siguió el ciclo de vida de un proyecto de Ciencia de Datos alineado con **DP-100**:
1. **Generación de Datos Sintéticos**: Simulación de 1,000+ registros con ruido operativo real.
2. **Preprocesamiento**: Codificación de variables categóricas y limpieza de datos.
3. **Entrenamiento**: Implementación de un modelo de clasificación (Random Forest).
4. **Validación**: Pruebas de estrés inyectando errores aleatorios para probar el sistema de alertas.

## 📈 Visualizaciones
El proyecto incluye un Dashboard Ejecutivo que presenta:
* Distribución de estados de portabilidad (Aprobados vs. Rechazados).
* Impacto de las alertas tempranas en la tasa de recuperación.
* Comparativa de tiempos de proceso con y sin optimización de IA.

## 🛠️ Tecnologías Utilizadas
* **Lenguaje**: Python (Google Colab).
* **Librerías**: Pandas, NumPy (Datos); Scikit-Learn (ML); Matplotlib, Seaborn (Visualización).
* **Model Deployment**: Joblib para la persistencia del modelo.
* **UI**: Formularios de Google Colab para la interacción en tiempo real.

## 🎓 Certificaciones Relacionadas
Este proyecto aplica dominios de **Microsoft Azure**:
* **AI-900 / DP-900**: Fundamentos de IA y gestión de datos Telco.
* **DP-100**: Diseño de soluciones de ciencia de datos y modelos predictivos.
* **AI-102**: Ingeniería de IA, automatización de procesos y manejo de errores operativos.

## 🏆 Resultados y Conclusiones
* **Precisión Predictiva**: El modelo logra anticipar rechazos con una alta tasa de confianza.
* **Eficiencia Temporal**: Reducción significativa en el tiempo promedio de portabilidad al automatizar la corrección de documentos.
* **Resiliencia**: El sistema es capaz de "salvar" trámites que normalmente fallarían por errores técnicos menores.

## 💼 Impacto para el Sector Empresarial
* **Reducción de Churn**: Al acelerar la portabilidad, se mejora la satisfacción del nuevo cliente.
* **Ahorro de Costos**: Menos intervención humana en validación de documentos y menos reprocesos.
* **Escalabilidad**: Capacidad de procesar miles de solicitudes simultáneas sin degradar el tiempo de respuesta.
