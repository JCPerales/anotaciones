#Configuracion prolog
En eclipse, instalar nuevo software, seleccion el plugin descargado

### Configurar perspectiva
Window/Perspective/Open/Other ... Seleccionar "Prolog Perspective"

### Configurar swipl
Eclipse/Preferencias/Prolog/Prolog Interpreters/ add/ SWI Prolog/ Browse `/usr/local/bin/swipl`

## Archivo de muestra criminal(X)

% Prolog File

%Ejemplo presentacion

criminal(X):-gringo(X),arma(Y),vende(X,Y,Z),hostil(Z).
enemigo(nono,gringos).
tiene(nono,m1).
misil(m1):-tiene(nono,m1).
vende(west,X,nono):-misil(X).
arma(X):-misil(X).
gringo(west).
hostil(X):-enemigo(X,gringos).


