# Introducción a tecnologías de Next Generation Sequencing (NGS)
Familarizarse con las diferentes tecnologías de Next Generation Sequencing 

# Instructora 👩‍🏫  
Thalía Araceli Silvestre Espejo 

Yo amo 🎤, 💃 and ☕


# Breve historia de la secuenciación del ADN
Resaltar hechos importantes antes de la comercialización de tecnologías de Next Generation Sequencing (NGS) en una línea de tiempo

<p align="center">
<img src="project-2021-05-20_10-05_AM.jpg" width="700" height="990" >

# Tecnologías de Next Generation Sequencing

```
Describe colectivamente los enfoques de secuenciación que han reducido el tiempo y el costo y han aumentado enormemente la producción de la secuencia en comparación con la secuenciación de Sanger. 
Tecnologías de secuenciación de alto rendimiento.
```
* NGS se caracteriza por realizar de millones a miles de millones de reacciones de secuenciación individuales simultáneamente en un proceso denominado secuenciación masivamente paralela.

* El enfoque ha revolucionado la secuenciación del ADN hasta el punto de que ahora se puede secuenciar un genoma humano completo en 3 días por alrededor de 1.000 dólares

 La siguiente figura representa la reducción de costo de secuenciamiento por megabases hasta agosto del 2020 de acuerdo a *National Human Genome
Research Institute (NHGRI)*
<p align="center">
<img src="https://www.genome.gov/sites/default/files/inline-images/NHGRISequencing_Cost_per_Megabase_Aug2020.jpg"  width="650" height="600">
 
 # Tecnologías de la segunda generación
 
```
Se describe como tecnologías de short-reads
```
**454**
 ```
  Esta tecnología está basada en el método de secuenciamiento por síntesis que involucra una combinación de PCR en emulsión y el pirosecuenciamiento
  ```
  2005 ➡️ Secuenciamiento y ensamblaje de *novo* del genoma de *Mycoplasma genitalium* con 96% de cobertura y 99,96% de presición en un corrida
  
 El pirosecuenciamiento se realiza usando una sola hebra de ADN de la muestra, cebador, enzima polimerasa, ATP sulfurilasa, luciferasa y apirasa como se muestra  en la siguiente figura. 

<p align="center">
<img src="https://github.com/bioinfoperu/Introduccion_Next_Genetarion_Sequencing/blob/main/Start-Here!.png" width="450" height="450">
 
| PLATAFORMA | PREPARACION DE LIBRERÍA | QUÍMICA | LONGITUD DE LECTURA | BASES POR CORRIDA | DURACION |
| ------------ | ------------- | ------------ | ------------- | ------------ | ------------- |
| Sanger |	PCR y clonación	| Fluoróforos	| 800	|800 pb	|3 horas |
| Roche 454 GS FLX Titanio |	PCR en emulsión	| Pirosecuenciación	| 400	| 500 Mb	| 10 h |
 
 
* Desventajas
  - Dificultad de interpretar el número de bases de un homopolímero
  - Producción de réplicas artificiales 
  - Costoso 
 
 
**ABI SOLiD**
 
 ```
  Esta tecnología está basada en ligación, usando el sitema de codificación di-base
  ```
 En la siguiente imagen estraída de Kürekçi et.al 2014 se podrá ver la metodología de secuenciamiento de manera detalla.
 Esta metodología inicia con la formación de librerías, unión de librerías a adaptadores que entan en perlas para proceder a la PCR en emulsión y continuar con el secuencimiento.
 El secuencimiento toma lugar con cebador universal (4 tipos), ligasa, sonda de 8-mers marcado con fluorescente en el extremo final.
 
<img src="https://github.com/bioinfoperu/Introduccion_Next_Genetarion_Sequencing/blob/main/solid.png" >
 
| PLATAFORMA | PREPARACION DE LIBRERÍA | QUÍMICA | LONGITUD DE LECTURA | BASES POR CORRIDA | DURACION |
| ------------ | ------------- | ------------ | ------------- | ------------ | ------------- |
| Sanger |	PCR y clonación	| Fluoróforos	| 800	|800 pb	|3 horas |
| Roche 454 GS FLX Titanio |	PCR en emulsión	| Pirosecuenciación	| 400	| 500 Mb	| 10 h |
|SOLiD	| PCR en emulsión |	Secuenciación por ligación |	50 |	30–50 Gb |	7-14 días |

* Ventaja
  - Secuencia una base dos veces lo que permite lograr una precisión general superior a 99,94%.
 
* Desventaja
  - Las herramientas bioinformpaticas se basan en llamadas de ADN en lugar de espacio de color.
  
**Illumina**
 
 ```
  Basada en secuenciación por síntesis, mediante el método método de terminación cíclica reversible.
 ```
 La fase de amplificación difiere de los dos anteriores tecnologías, Illumina se basa en PCR puente.
 El secuenciamiento comienza con la adición de cebador, ADN polimerasa y diferentes nucleótidos terminadores marcados con fluorescencia. 
 Con la adición de cada nucleótido, la síntesis se detiene y se registra la luz de fluorescencia. Después de la eliminación del grupo químico terminador que está conectado al nucleótido, tiene lugar el siguiente ciclo de síntesis.
 
 <img src="https://github.com/bioinfoperu/Introduccion_Next_Genetarion_Sequencing/blob/main/ilunina.png">
 Figura extraída de Low et al. 2017
 
 La plataforma Illumina posee diferentes sistemas de secuenciación tal como se muestra en la siguiente tabla estraída de Kumar et al. 2019
 
 <img src="https://github.com/bioinfoperu/Introduccion_Next_Genetarion_Sequencing/blob/main/tabla:illu.png">
 
| PLATAFORMA | PREPARACION DE LIBRERÍA | QUÍMICA | LONGITUD DE LECTURA | BASES POR CORRIDA | DURACION |
| ------------ | ------------- | ------------ | ------------- | ------------ | ------------- |
| Sanger |	PCR y clonación	| Fluoróforos	| 800	|800 pb	|3 horas |
| Roche 454 GS FLX Titanio |	PCR en emulsión	| Pirosecuenciación	| 400	| 500 Mb	| 10 h |
|SOLiD	| PCR en emulsión |	Secuenciación por ligación |	50 |	30–50 Gb |	7-14 días |
| Illumina |	PCR	Puente | Terminadores reversibles |	35-300	| 0,1–3000 Gb | 7 a 84 h |
 
* Ventajas
  - Bajo Costo
  - Herramientas bioinformticas para procesar la data 
  - No tiene problemas con los homopolimeros 
  - Reads en paired-end
 
* Desventajas 
  - El extremo 3' de los reads tienen baja calidad.
  - Errores en las regiones invertidad repetidas y secuencias GCC.
  - Cualquier burbuja o daño en elos reactivos influencia negativamente en el secuenciamiento.

 **Ion Torrent**
 
 ```
 Se basa en la detección de el ión de hidrógeno liberado durante el proceso de secuenciación.
 ```
 En la siguiente imagen de Kchouk et al. 2017 se explica el proceso de secuenciación.
 
<p align="center">
 <img src="https://github.com/bioinfoperu/Introduccion_Next_Genetarion_Sequencing/blob/main/ion.png">
 
 
 | PLATAFORMA | PREPARACION DE LIBRERÍA | QUÍMICA | LONGITUD DE LECTURA | BASES POR CORRIDA | DURACION |
| ------------ | ------------- | ------------ | ------------- | ------------ | ------------- |
| Sanger |	PCR y clonación	| Fluoróforos	| 800	|800 pb	|3 horas |
| Roche 454 GS FLX Titanio |	PCR en emulsión	| Pirosecuenciación	| 400	| 500 Mb	| 10 h |
|SOLiD	| PCR en emulsión |	Secuenciación por ligación |	50 |	30–50 Gb |	7-14 días |
| Illumina |	PCR	Puente | Terminadores reversibles |	35-300	| 0,1–3000 Gb | 7 a 84 h |
| Ion Torrent| PCR en emulsión | Detección de iones de hidrógeno | 200-500| 10 Gb| 2 a 8|

* Ventajas
  - Bajo Costo
  - Rápido
  - Longitud de Lecturá más grande en comparción de las otras tecnología de NGS  de segunda generación
 
* Desventajas 
  - Difícil detección de homopolímeros.
  - No es tan preciso.
 
# Tecnologías de la tercera generación

 ```
Se describe como tecnologías de long-reads
```
 Secuenciamiento en tiempo real.
 
 Secuenciamiento rápido.
 
 **Pacific Biosciences**
  ```
Pacific Biosciences realizó 2 principales innovaciones que permitieron observar el secuenciamiento de una sola molécula de ADN en tiempo real.
Los nucleótidos fosfomarcados con fluorescentes y zero-mode waveguide (ZMW), secuenciamiento por síntesis 
```
  <img src= "https://ars.els-cdn.com/content/image/1-s2.0-S1672022915001345-gr3.jpg">
 Road et al. 2015
 
 * Ventajas
  - Observar la actividad cinética de la ADN polimeraza. 
  - Reads de hasta 10-15Kb.
 
* Desventajas 
  - Costoso.
  - Tasa de error entre 10 a 15%.
 
 **Oxford Nanopore Technologies**
   ```
 Detección de nucleótidos miestras el ADN pasa a través del nanopore, utilizando la tecnología de interrupción de la corriente.
 ```
 <img scr= "https://github.com/bioinfoperu/Introduccion_Next_Genetarion_Sequencing/blob/main/nano.png">
 He et. al 2021
 
* Ventajas 
  - Asequible.
  - Portable
* Desventajas 
  - Alta tasa de error.
 
 # Referencias
 
He, M., Chi, X., & Ren, J. (2021). Applications of Oxford Nanopore Sequencing in Schizosaccharomyces pombe. In Yeast Protocols (pp. 97-116). Humana, New York, NY.
  
Kchouk, M., Gibrat, J. F., & Elloumi, M. (2017). Generations of sequencing technologies: from first to next generation. Biology and Medicine, 9(3).
 
Kumar, K. R., Cowley, M. J., & Davis, R. L. (2019, October). Next-generation sequencing and emerging technologies. In Seminars in thrombosis and hemostasis (Vol. 45, No. 07, pp. 661-673). Thieme Medical Publishers.
 
 Kürekçi, G. K., & Dinçer, P. (2014). Next-Generation DNA Sequencing Technologies. Erciyes Medical Journal/Erciyes Tip Dergisi, 36(3).
 
Low, L. W. Y., & Tammi, M. T. (Eds.). (2017). Bioinformatics: A Practical Handbook of Next Generation Sequencing and Its Applications. 
 
Rhoads, A., & Au, K. F. (2015). PacBio sequencing and its applications. Genomics, proteomics & bioinformatics, 13(5), 278-289.
 
