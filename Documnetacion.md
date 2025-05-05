
### Documantacion del csv:

## Base de datos de eventos de emergencia de desastres naturales
Desastres naturales globales entre 1900 y 2022

El conjunto de datos EM-DAT - Country Profiles proporciona cifras agregadas de desastres naturales en EM-DAT, que es la base de datos de eventos de emergencia, mantenida por el Centro de Investigación sobre Epidemiología de Desastres (CRED). El conjunto de datos incluye datos sobre el número de desastres, el número total de personas afectadas, el número total de muertes y las pérdidas económicas (valor original y ajustadas) para diferentes subtipos de desastres para cada país y año. El conjunto de datos contiene información sobre desastres naturales de todo el mundo.

## Columnas:

- Año: El año en el que ocurrió el desastre.
- País: El país donde ocurrió el desastre.
- Subtipo de desastre: El tipo de desastre (por ejemplo, inundación, terremoto, tormenta, sequía).
- Número de desastres: El número total de desastres que ocurrieron en un año determinado para un país específico y subtipo de desastre.
- Afectado total: El número total de personas afectadas por el desastre en un año determinado para un país específico y subtipo de desastre.
- Muertes totales: El número total de muertes resultantes del desastre en un año determinado para un país específico y subtipo de desastre.
- Pérdidas económicas totales (original): Las pérdidas económicas totales resultantes del desastre, en la moneda original del país, en un año determinado para un país específico y subtipo de desastre.
- Pérdidas económicas totales (ajustadas): Las pérdidas económicas totales resultantes del desastre, ajustadas por inflación y expresadas en dólares estadounidenses de 2019, en un año determinado para un país específico y subtipo de desastre.

Year: Año en el que ocurrió el desastre natural.


Country: País donde ocurrió el desastre.


ISO: Código ISO del país.


Disaster Group: Grupo del desastre (por ejemplo, geofísico, meteorológico, etc.).


Disaster Subgroup: Subgrupo dentro del tipo de desastre (por ejemplo, terremoto, huracán, etc.).


Disaster Type: Tipo general de desastre (ej. terremoto, inundación).


Disaster Subtype: Subtipo del desastre (más específico que el tipo).


Total Events: Número total de eventos (pueden ser múltiples eventos en un solo desastre).


Total Affected: Número total de personas afectadas.


Total Deaths: Número total de muertes.


Total Damage (USD, original): Daños totales en USD según el valor original.


Total Damage (USD, adjusted): Daños totales en USD ajustados (probablemente por inflación u otros factores).


CPI: Índice de Precios al Consumidor.



## Volumen de datos:

El conjunto de datos contiene múltiples filas de datos para cada combinación de año, país y subtipo de desastre, que abarcan desde 1900 hasta 2022. El conjunto de datos tiene un total de 47.682 filas y 8 columnas.

## Fuente:

El conjunto de datos proviene del Centro de Investigación sobre la Epidemiología de Desastres (CRED), que forma parte de la Universidad de Lovaina en Bruselas, Bélgica.



---------------------------------------

## Tipos de Desastre y su Significado

| Tipo de Desastre               | Traducción al Español               | Descripción                                                    |
|----------------------------------|-------------------------------------|-----------------------------------------------------------------|
| **Insect infestation**           | plagas de insectos                 | Plagas de insectos que afectan cultivos, ecosistemas o salud humana (ej.: langostas,mosquitos transmisores de enfermedades). | 
| **Drought**                      | Sequía                             | Periodos prolongados de escasez de agua que afectan cultivos, ganado y abastecimiento de agua. |
| **Volcanic activity**            | Actividad volcánica                | Erupciones, emisiones de ceniza o lava, explosiones volcánicas. |
| **Wildfire**                     | Incendio forestal                  | Fuegos no controlados en bosques, praderas o zonas rurales.     |
| **Flood**                        | Inundación                         | Acumulación de agua que cubre zonas que normalmente están secas (ríos desbordados, lluvias extremas). |
| **Storm**                        | Tormenta                           | Fenómenos meteorológicos severos con fuertes vientos, lluvia, granizo, o tormentas tropicales y huracanes. |
| **Extreme temperature**          | Temperaturas extremas              | Olas de calor o frío intenso que pueden causar impactos en salud, agricultura y energía. |
| **Earthquake**                   | Terremoto                          | Movimiento sísmico del suelo causado por la actividad tectónica. |
| **Mass movement (dry)**          | Movimiento de masas (en seco)      | Deslizamientos de tierra, derrumbes o colapsos de terreno sin presencia de agua. |
| **Landslide**                    | Deslizamiento de tierra            | Movimiento de masas de tierra, rocas o escombros, a menudo debido a lluvias intensas o terremotos. |
| **Animal accident**              | Accidente con animales            | Accidentes provocados por animales (ej.: estampidas, ataques de fauna). Muy poco frecuente. |
| **Fog**                          | Niebla                             | Fenómenos de niebla intensa que pueden provocar accidentes, especialmente de tráfico. |
| **Glacial lake outburst**        | Desbordamiento de lago glaciar     | Liberación repentina de grandes cantidades de agua de un lago glaciar, lo que puede causar inundaciones destructivas. |






----------------------------------------

## Decisiones

Columnas: Total Damage (USD, original) y Total Damage (USD, adjusted)  --->>> decidimos quedarnos con Total Damage (USD, adjusted) ya que ambas indican lo mismo pero esta columna  esta ajustada a la invlación y está en Dolares, ya que vamos a comparar eventos de diferentes años y de diferentes países, por lo que comparar daños sin ajustar la inflacion no seria correcto ya que el valor del dinero cambia con el tiempo.