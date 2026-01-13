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



## 🔍 Insights Principales
Existe un 6% de Fraude. 

Days_Policy_Accident none                   16.4 
 4 AgeOfPolicyHolder    21 to 25            14.8 
 5 Days_Policy_Claim    8 to 15            14.3 
 6 PolicyType           Sport - Collision   13.8 
 7 VehicleCategory      Utility                11.3 
 8 BasePolicy           All Perils           10.2 
 9 VehiclePrice         less than 20000     9.40
10 AgeOfVehicle         4 years              9.17


