# Rotacional y Divergencia

![Ej2](https://user-images.githubusercontent.com/44282912/213842957-cf969b58-f74d-434e-9262-bc5886272548.png)

Programa que permite el graficado del rotacional y la divergencia en un campo vectorial. Además nos permite visualizar el efecto que tiene este campo sobre una curva que se posiciona en este campo.

## Uso

Para su uso tenemos que:  

  - Poner nuestra función del campo vectorial en su forma $M(x,y)$ y $N(x,y)$ en la primer pestaña (`Campo`) del panel de `Entrada`
  - Cambiar a la pestaña de `Curva` si requerimos ver como interactúa una curva paramétrica en este campo vectorial
  - Ir a la sección de `Salida` de la aplicación y ajustar los controles del gráfico como sea necesario
  - Tanto en la pestaña de `Curva` de esta sección como en el fondo de la misma podemos seleccionar que elementos deseamos graficar
  - Presionar el botón de `Graficar`
  
![imagen](https://user-images.githubusercontent.com/44282912/213845122-535e9854-a42e-4f60-965f-42362743a9d6.png)

## Más ejemplos

Algunos ejemplos de funciones $M(x,y)$ y $N(x,y)$ que se pueden probar son:
Ejemplos adicionales que pueden probar, M(x,y) y N(x,y) están separadas por comas:

```matlab
F = [ x.^2-y.*x, y.^2-x.*y];
F = [ cos(x+2.*y), sin(x-2.*y) ];
F = [ -y,x ];
F = [ (2.*x).*(exp(x.*y))+(x.^2).*(y).*(exp(x.*y)), (x.^3).*(exp(x.*y))+2.*y ];
F = [ 2.*x, 2.*y ];
F = [ 2.*x.^3.*y.^4+x, 2.*x.^4.*y.^3+1];
F = [ x.^3-4.*x.*y.^2+2, 6.*x-7.*y+x.^3.*y.^3];
F = [ 2.*x.*sin(2.*y)-3.*y.^2, 2-6.*x.*y+2.*x.^2.*cos(2.*y)];
F = [ 6-2.*x.*y+y.^3, x.^2-8.*y+3.*x.*y.^2];
F = [ y.^2+y.^2.*cos(x+y), 2.*x.*y-2.*y+y.^2.*cos(x+y)+2.*y.*sin(x+y) ];
```

## Disclaimer

El programa se escribió en Matlab R2019a pero se probó compatibilidad con R2020 y R2022, no debería de haber problema con esta aplicación mientras se tenga una versión reciente que tenga el componente `Matlab App Designer`.
