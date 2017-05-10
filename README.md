# Sistema Experto - Seleccion Proveedores
Sistema experto basado en reglas que con base en la configuración de las mismas en un formato de CLIPS, se utiliza este motor para el desarrollo del problema.

## Objetivo
El sistema debe,por medio de una serie de reglas configuradas en el archivo .clp ejecutarlas y determinar el porcentaje que calificará a los proveedores con base en los criterios definidos.

## Criterios

### Cost
    Evaluará el costo del producto del proveedor, sus dimensiones son:

	ProductPrice
	Freight cost
	Tariff and custom duties

### Quality	
    Evaluará la calidad del producto del proveedor, sus dimensiones son:

	Rejection rate of the product
	Increased lead time
	Quality assesment
	Remedy for quality problems

### ServicePerformance	
    Evaluará el desempeño del proveedor respecto a las necesidades de la organización, sus dimensiones son:

	Delivery schedule
	Technological and R&D support
	Response to changes
	Ease of communication

### Supplier's profile
    Evalúa el perfil del proveedor, lo que tiene que ver con las características del proveedor que finalmente afectan a la organización:

	Finnancial status
	Customer base
	Performance history
	Production facility and capacity
	Geographical location
	Political stability
	Economy
	Terrorism

## Business Logic

El sistema experto tomará los datos en cada una de las dimensiones y realizará una evaluación del criterio. Por ejemplo, para "Cost", se evaluarán "ProductPrice",	"Freight cost" y "Tariff and custom duties", las cuales en conjunto darán la evaluación total del criterio.

Al evaluar los cuatro criterios la aplicación realizará una ponderación de la nota con base en el peso de cada uno de los criterios (peso que podrá ser parametrizado por el usuario).

