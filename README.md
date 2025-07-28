# Seguimiento_1
Seguimiento 1 de Bioinform??tica 2025-2 - An??lisis GFF3 de Vicugna pacos

## Punto n??1: Describa los campos que se encontrar?? en este tipo de archivos. ??Qu?? informaci??n est?? all?? contenida? Proporcione ejemplos.

R//: Los archivos GFF3 se usan para guardar informaci??n sobre diferentes partes del ADN, como genes, exones y otras regiones.  
Cada l??nea del archivo describe algo distinto del genoma y est?? dividida en 9 columnas, que est??n separadas por tabulaciones.  
Cada columna tiene un tipo de dato que sirve para identificar o clasificar esa informaci??n.

1. **Columna 1 ??? seqid**  
   Dice en qu?? secuencia del genoma est?? lo que se est?? describiendo.  
   Puede ser un cromosoma o una secuencia ensamblada.  
   *Ejemplo:* `ctg123`

2. **Columna 2 ??? source**  
   Es la fuente que gener?? la informaci??n. Por ejemplo, puede venir de una base de datos o un programa.  
   Esto ayuda a saber si viene de un lugar confiable.  
   *Ejemplo:* `GenBank`

3. **Columna 3 ??? type**  
   Muestra qu?? tipo de cosa se est?? describiendo: puede ser un gen, un ex??n o una regi??n codificante.  
   *Ejemplo:* `gene`, `exon`, `CDS`

4. **Columna 4 ??? start**  
   Indica desde qu?? posici??n comienza esa parte del ADN. Se empieza a contar desde 1.  
   *Ejemplo:* `1000`

5. **Columna 5 ??? end**  
   Muestra en qu?? posici??n termina.  
   *Ejemplo:* `9000`  
   Con las columnas 4 y 5 se puede saber la longitud del fragmento.

6. **Columna 6 ??? score**  
   Es un n??mero que indica qu?? tan confiable o fuerte es el dato. Si no hay valor, se pone un punto (`.`).  
   *Ejemplo:* `0.95` o `.`

7. **Columna 7 ??? strand**  
   Dice en qu?? hebra est??: `+` para la directa y `-` para la complementaria.  
   *Ejemplo:* `+`

8. **Columna 8 ??? phase**  
   Solo se usa si el tipo es `CDS`. Indica si el cod??n empieza en la primera, segunda o tercera base.  
   *Ejemplo:* `0`

9. **Columna 9 ??? attributes**  
   Tiene informaci??n adicional como el ID o el nombre del gen. Est?? escrita como clave=valor, separada por punto y coma.  
   *Ejemplo:* `ID=gene00001;Name=BRCA1`
   
## Punto n??2: DESCARGA DE ARCHIVOS DE TRABAJO
## Vaya a http://ftp.ensembl.org/pub/current_gff3/ para descargar el archivo GFF del organismo asignado.

## a. La descarga del archivo GFF debe ser mediante l??nea de comandos. Incluir el comando.
## c. Descomprima el archivo usando la l??nea de comandos. Incluir el comando

R//: El organismo que me correspondio fue el "Vicugna pacos". El archivo m??s general `Vicugna_pacos.vicPac1.114.gff3.gz` fue el que descargue. 
Use `wget para descargar`  el archivo y `gunzip` para descomprimirlo.

## Punto n??3:. AN??LISIS DEL ARCHIVO

## a. Proporcione una breve descripci??n del organismo asignado en el archivo README.

R//: Vicugna pacos es el nombre cient??fico de la alpaca. Es un mam??fero domesticado que se cr??a por su lana, especialmente en los Andes de Per??, Bolivia, Chile y el norte de Argentina. Pertenece a la misma familia que las llamas y las vicu??as, y est?? adaptada a vivir en zonas de gran altitud.

## b. Investigue, usando las herramientas de la l??nea de comandos de Unix, y conteste las siguientes preguntas:

## i. ??Cuantos features contiene el archivo?

R//: El archivo contiene 704184 features.  

## ii. ??Cuantas regiones de la secuencia (cromosomas) contiene el archivo?

R//: El archivo contiene 290927 regiones de la secuencia.

## iii. ??Cu??ntos genes est??n listados en el organismo?

R //: El archivo contiene 11765 genes listados.

## iv. ??Cu??l es el top 10 de tipo de features (columna 3) m??s anotados en el genoma?

R//: Los 10 tipos de features m??s anotados en el archivo son:
1. scaffold ??? 287207
2. exon ??? 154363
3. CDS ??? 147331
4. biological_region ??? 81132
5. mRNA ??? 11806
6. gene ??? 11765
7. region ??? 3720
8. ncRNA_gene ??? 2532
9. snRNA ??? 993
10. pseudogenic_transcript ??? 898






