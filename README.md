# 🚗 Car Insurance Fraud Detection

El objetivo del proyecto es **predecir si una reclamación de seguro automotor es fraudulenta**, analizando patrones demográficos, características del vehículo y condiciones del siniestro.

---

## 📊 Dataset

📦 Fuente: [Insurance Company Benchmark (Car Claims) – Kaggle / UCI]  
El dataset contiene información detallada sobre **reclamos de seguros de automóviles**, incluyendo datos del asegurado, vehículo, tipo de póliza y siniestros reportados.

**Variables principales:**
- `Month`, `WeekOfMonth`, `DayOfWeek` → Fecha y periodicidad del reclamo  
- `Make`, `VehicleCategory`, `VehiclePrice` → Marca, tipo y valor del vehículo  
- `AccidentArea` → Zona donde ocurrió el accidente (urbana o rural)  
- `Sex`, `MaritalStatus`, `Age`, `AgeOfPolicyHolder` → Datos demográficos  
- `PolicyType`, `BasePolicy`, `Fault` → Información de la póliza  
- `Deductible`, `DriverRating` → Métricas del conductor y póliza  
- `Days_Policy_Accident`, `Days_Policy_Claim` → Días entre eventos  
- `PastNumberOfClaims`, `NumberOfSuppliments`, `PoliceReportFiled`, `WitnessPresent` → Variables sobre reclamos previos y reportes  
- `FraudFound_P` → Variable objetivo (1 = fraude detectado, 0 = legítimo)

---

## 🧹 Limpieza de datos

---- ✅ Sin valores faltantes significativos.  
- ⚠️ Outliers en `Deductible` y `DriverRating` verificados mediante análisis de caja.  
- Codificación de variables categóricas y normalización de numéricas.  
- División en **train/test (80/20)** para modelado y validación.


## 🔍 Insights Principales

### 🧑‍💼 Demografía
- **Hombres jóvenes (16–25 años)** y **viudos** presentan **mayor probabilidad de cometer fraude**.  

### 🚘 Vehículo
- **Autos nuevos o de 3 a 5 años** muestran más casos fraudulentos.  
- **Sedans y vehículos utilitarios** son las categorías con más fraudes.  
- Marcas con más incidencia: **Accura, Mercedes, Saab, Saturn**.  
- **Vehículos muy baratos o muy caros** concentran la mayoría de los fraudes.

### ⚙️ Póliza y reclamo
- Si **el accidente fue culpa del asegurado**, la probabilidad de fraude aumenta significativamente.  
- Tipos de póliza con más fraudes: **All Perils** y **Collision**.  
- Reclamos **sin reporte policial ni testigos** son **altamente sospechosos**.  


