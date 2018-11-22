# Proyecto RES2+U - Sensorización
Aquí se encuentran alojados los datos recogidos por los sensores de las diferentes plataformas involucradas en el proyecto RES2+U.

La actualización se realiza diariamente en las respectivas ramas que representan cada una de las plataformas de sensorizaciones y semanalmente en la rama estable master.

## Prerrequisitos
Tener instalado Git y GitHub. Hay muchos tutoriales en Internet que muestran el proceso de instalación en función del sistema operativo que se tenga.

## Comenzando
Los comandos utilizados en los scripts correspondientes a cada plataforma son los mostrados a continuación. 

Algunos de ellos incluyen las letras "XXXXXXXXXX", en su lugar se debe poner smartcei, edificacion, minas o itd en función de la plataforma que se trate. Por ejemplo, si usted es el encargado de la plataforma de la E.T.S. de Edificación (ETSEM) deberá incluir en el lugar de "XXXXXXXXXX" "edificacion". Son todos en minúsculas y sin tildes.

Con el siguiente comando se generará una carpeta llamada RES2+U_XXXXXXXXXX en el directorio sobre el que se esté posicionado y desde la que se generará el acceso a la plataforma donde se alojan los datos recogidos por los sensores

```
git clone https://github.com/soniasc18/RES2-U RES2+U_XXXXXXXXXX
```

Para desplazarse por los directorios:
```
cd RES2+U_XXXXXXXXXX
```

Este comando sirve para crear la rama sobre la que se trabajará de aquí en adelante, su nombre es XXXXXXXXXX
```
git checkout -b XXXXXXXXXX
```

Para crear carpetas de nombre XXXXXXXXXX
```
mkdir XXXXXXXXXX
```
Ahora vamos dentro de ella para poder incluir ahí los ficheros .csv
```
cd XXXXXXXXXX
```

Los siguientes comandos realizan la subida de dichos ficheros ubicados en la carpeta RES2+U_XXXXXXXXXX/XXXXXXXXXX a la plataforma de GitHub. <AAAA/MM/DD> corresponde con la fecha del día en concreto, por ejemplo 2018/09/19.
```
git add .
git commit -m "Datos XXXXXXXXXX <AAAA/MM/DD>"
git push origin XXXXXXXXXX
```
