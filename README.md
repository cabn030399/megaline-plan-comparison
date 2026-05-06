# Análisis de Tarifas Megaline 📊

Descripción del Proyecto
Este proyecto analiza el comportamiento de usuarios y la rentabilidad de dos planes de telecomunicaciones de la empresa Megaline: Surf y Ultimate. El objetivo principal es determinar cuál de las dos tarifas genera más ingresos para optimizar el presupuesto de publicidad.

🎯 Objetivos
Analizar el comportamiento de 500 clientes de Megaline durante 2018
Comparar el uso de servicios (llamadas, mensajes, internet) entre ambos planes
Calcular los ingresos mensuales por usuario considerando excesos de consumo
Determinar qué plan es más rentable para la empresa
Realizar pruebas estadísticas para validar las diferencias encontradas
📋 Estructura de Datos
El análisis utiliza 5 datasets principales:

### 1. Usuarios (megaline_users.csv)
- Información demográfica y plan contratado
- Fechas de registro y cancelación

### 2. Llamadas (megaline_calls.csv)
- Registro detallado de llamadas por usuario
- Duración y fechas de las llamadas

### 3. Mensajes (megaline_messages.csv)
- Historial de mensajes SMS enviados
- Fechas de envío por usuario

### 4. Internet (megaline_internet.csv)
- Consumo de datos móviles por sesión
- Volumen en MB por usuario y fecha

### 5. Planes (megaline_plans.csv)
- Detalles de las tarifas Surf y Ultimate
- Límites incluidos y costos por exceso

🔧 Tecnologías Utilizadas
Python 3.9+
Pandas
Manipulación y análisis de datos
NumPy
Operaciones matemáticas
Matplotlib & Seaborn
Visualización de datos
SciPy
Pruebas estadísticas
Jupyter Notebook
Desarrollo interactivo
📊 Metodología
### 1. Preparación de Datos
- Limpieza y corrección de tipos de datos
- Manejo de valores faltantes
- Conversión de fechas y unidades

### 2. Análisis Exploratorio
- Estadísticas descriptivas por plan
- Visualizaciones comparativas
- Identificación de patrones de uso

### 3. Cálculo de Ingresos
- Aplicación de reglas de redondeo (minutos y GB hacia arriba)
- Cálculo de excesos y cargos adicionales
- Estimación de ingresos mensuales por usuario

### 4. Pruebas Estadísticas
- Comparación de ingresos promedio entre planes
- Análisis regional (NY-NJ vs otras regiones)
- Pruebas t de Student para validar diferencias

🎨 Visualizaciones Incluidas
Histogramas de distribución de uso por plan
Diagramas de caja para comparar comportamientos
Gráficos de barras para promedios mensuales
Análisis de tendencias temporales

📈 Principales Hallazgos
Comportamiento de Usuarios por Plan
Llamadas:
- Ambos planes muestran una duración promedio de llamadas muy similar (~6.5 minutos)
- Los usuarios de Ultimate no aprovechan completamente sus 3000 minutos incluidos
- El promedio de uso mensual es de ~410 minutos para ambos planes
- Los usuarios de Surf ocasionalmente exceden su límite de 500 minutos

Mensajes:
- Los usuarios de Ultimate envían más mensajes en promedio (46.3 SMS/mes vs 40.1 SMS/mes)
- El plan Surf tiene mayor variabilidad en el uso de mensajes
- Ambos planes están generalmente dentro de sus límites incluidos

Internet:
- Consumo promedio muy similar entre planes (~40-41 GB/mes)
- Los usuarios de Surf frecuentemente exceden su límite de 15 GB
- Los usuarios de Ultimate raramente exceden su límite de 30 GB

Análisis de Ingresos
Plan Ultimate:
- Ingreso promedio: $72.25/mes
- Mayor estabilidad (baja variabilidad)
- Ingresos más predecibles debido a menos excesos

Plan Surf:
- Ingreso promedio: $60.42/mes
- Alta variabilidad ($20 - $590.37/mes)
- Ingresos impredecibles debido a frecuentes excesos

Pruebas Estadísticas
Diferencia de ingresos entre planes: 
Existe diferencia estadísticamente significativa (p < 0.05)
Ultimate genera $11.83 más en promedio por usuario
Diferencia regional (NY-NJ vs Otras):
Diferencia estadísticamente significativa (p = 0.0104)
Los usuarios de NY-NJ generan menores ingresos promedio
Recomendación Estratégica
El Plan Ultimate es más rentable para la empresa porque:
- Genera mayor ingreso promedio por usuario
- Ofrece ingresos más estables y predecibles
- Los usuarios consumen menos de lo incluido, maximizando la rentabilidad
- Menor costo de atención al cliente por excesos

Recomendación: Enfocar el presupuesto publicitario en promover el Plan Ultimate, especialmente dirigido a usuarios que consumen moderadamente los servicios.
