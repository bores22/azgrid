2012/06/26
Componente QuadGrid para Unity3D
V. 01
por Cesar Pach�n (http://www.cesarpachon.com) 

sitio del proyecto: https://github.com/cesarpachon/azgrid
sitio de la compa��a: http://www.cesarpachon.com

RESUMEN
QuadGrid es un sencillo componente para Unity3D que permite la creaci�n y edici�n de una cuadr�cula bidimensional. 
Se enfoca en ser sencillo y ligero.
En particular, s�lo consume un GameObject. no crea GameObjects separados para cada celda. 
Soporta las siguientes caracter�sticas:
1. visualizaci�n y edici�n en modos EDICION y EJECUCION de Unity3D.
2. materiales separados para celdas y l�neas.
3. mostrar/ocular celdas � lineas.
4. cambiar el ancho/alto de las celdas.
5. cambiar el ancho de la l�nea de separaci�n.
6. generar eventos OnTouchedCell
7. funciona a�n si la cuadricula es rotada, escalada, o cambia de posici�n.


IMPLEMENTACION
Est� implementada utilizando dos mallas generadas proceduralmente. para dibujar utiliza el m�todo Graphics.DrawMesh.

USO
Debes crear un GameObject vac�o, y asociarle el script AZQuadGrid.
En el inspector, puedes asignarle materiales, configurar el n�mero de filas y columnas, cmabiar el ancho y el alto..
si quieres recibir eventos, asocia un script propio que tenga un m�todo as�: 
 public void OnTouchedCell(AZQuadGrid.AZQuadCell cell)
la estructura cell que se recibe por par�metros contiene la fila y la columna seleccionada, as� como el centro de la celda como un Vector3.

EJEMPLO
Verifica la escena de ejemplo que acompa�a este paquete.

DOCUMENTACION
verifica el video de presentaci�n en  https://www.youtube.com/watch?v=ecupnLGvWAI

LICENCIA Y GARANT�A
Todo el c�digo est� licenciado bajo LGPL V3


