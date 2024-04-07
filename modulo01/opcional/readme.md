# Bakend relacional. Laboratorio 1.
## Opcional

Para el enunciado opcional realizo el diagrama entidad relacion.

### Entidades
Tengo 6 entidades: Cursos, Autores, Articulos, Videos, Tematicas (Topics), Usuarios.

### Relaciones
* Un curso siempre tiene uno o muchos articulos, pero  al menos tiene siempre un articulo. Un articulo debe estar siempre dentro de un curso, no voy a tener articulos sueltos que no pertenezcan a ningun curso.

* Un curso siempre va a tener un autor principal. Se supone que el es quien escribe los articulos del curso. Sin embargo, puede que yo tenga un autor que no sea el autor principal de ningun curso.

* Un curso puede tener ninguno, uno o muchos videos. Pero un video siempre debe pertenecer a un curso.

* Un curso siempre tiene una tematica, pero puede haber tematicas que no tengan ningun curso asociado.

* Un video siempre tiene un autor. Un autor puede tener ninguno, uno o muchos videos. 

* Un video siempre tiene una tematica. Una tematica puede estar en ninguno, uno o muchos videos. 

* Una tematica puede tener una tematica padre, o ninguna (en el caso de ser una tematica principal). Una tematica puede tener ninguna, una o muchas tematicas subordinadas (o hijas).

* Distinguimos los videos publicos de los privados mediante un campo booleano IsPublic.

* Un video puede estar asociado a uno o varios tags. Un mismo tag puede figurar en varios videos. Tenemos una relación N a N. Como además cada video aparece en un solo curso, cada curso queda asociado a los tags de sus videos.

* Distinguimos los usuarios normales de los suscriptores por el campo booleano IsSuscriptor en el usuario.

* En todo caso un usario puede tener muchos cursos, y un curso será segudio por muchos usarios. Es una relación N a N. Tenemos entonces la entidad intermedia UserCourse. Este entidad tiene además datos adicionales sobre la relación, como el progreso del usuario dentro de ese curso.

* Las visualizaciones de los videos. Según el enunciado entiendo que son las visualizaciones que un video ha tenido por parte de todos los usuarios. Por ello cada video tendra un campo ViewedCounter. 

* Si quiero un total de visualizaciones para todos los videos de un curso, pues también pudo tener un campo en el curso que tenga la suma de todas las visualizaciones, TotalViewdCounter, aunque este campo podria ser redundante, bastaria con recorrer las visualizaciones d elos videos de ese curso.

