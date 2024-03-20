# Bakend relacional. Laboratorio 1.
## Basico

Para el enunciado basico realizo el diagrama entidad relacion.

### Entidades
Tengo 5 entidades: Cursos, Autores, Articulos, Videos, Tematicas (Topics).

### Relaciones
Un curso siempre tiene uno o muchos articulos, pero  al menos tiene siempre un articulo. Un articulo debe estar siempre dentro de un curso, no voy a tener articulos sueltos que no pertenezcan a ningun curso.
---
Un curso siempre va a tener un autor principal. Se supone que el es quien escribe los articulos del curso. Sin embargo, puede que yo tenga un autor que no sea el autor principal de ningun curso.
---
Un curso puede tener ninguno, uno o muchos videos. Pero un video siempre debe pertenecer a un curso.
---
Un curso siempre tiene una tematica, pero puede haber tematicas que no tengan ningun curso asociado.
---
Un video siempre tiene un autor. Un autor puede tener ninguno, uno o muchos videos. 
---
Un video siempre tiene una tematica. Una tematica puede estar en ninguno, uno o muchos videos. 
