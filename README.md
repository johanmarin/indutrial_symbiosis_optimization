# indutrial_symbiosis_optimization

![Huella concreto](https://cdn.ticbeat.com/src/uploads/2019/12/huella-carbono-cemento-600x428.jpg)

## Contexto
Con el objetivo de disminuir la emisión de CO2 algunas empresas cementeras han decidido sustituir 
parte del cemento, por materiales cementantes suplementarios más amigables con el medio ambiente,
en la preparación del concreto. 

Uno de estos materiales es la ceniza de cascarilla de arroz (CCA). Sin embargo si se tiene en cuenta
el transporte de CCA hasta las cementeras, pueden presentarse casos en que se da el caso contrario y
el transporte de este material aumenta las emisiones de CO2 totales.Con el fin de evaluar la 
viabilidad de esta opción en Colombia, se desarrolla un modelo de optimización lineal, implementado
en Python y solucionado utilizando el solver [CPLEX](https://www.ibm.com/co-es/analytics/cplex-optimizer) 
de IBM. 

Para el problema se tenía un total de 7 cementeras
  + Rioclaro
  + Yumbo
  + Tolú viejo
  + Cartagena
  + Sogamoso 
  + Montebello
  + Nare
  
 4 concreteras 
  + Barranquilla
  + Flandes 
  + Fusagasugá
  + Puerto Tejada
 
 2 Trilladoras de Arroz
  + Valledupar 
  + Yopal
  
 ## Escenarios
 
 ### Escenario base
 El proceso se realiza normalmente sin sutitución de material cementante por CCA
 
 ### Transformación en fuente
 Se produce cascarilla de arroz se transforma en CCA  en cada trilladora 
 y se transportan hasta cada una de las concreteras.
 
 
 ### Tranformación centralizada
 Se tiene un centro de distribución que agrupa la cascarilla de arroz que se envía sin procesar 
 desde las trilladoras, allí se procesa en CCA y se envía a las plantas de concreto. 
 Para este escenario se realizó un modelo en el que se cambió la localización del centro de distribución,
 evaluando 4 posibilidades seleccionadas arbitrariamente en la zona central del país
 
  + Fusagasugá
  + Ibagué
  + Tunja
  + Yopal

 
 
 
