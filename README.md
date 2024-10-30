# ZIPCRACK - Ataque de Diccionario a Archivos ZIP

**Versión:** 1.0.1  
**Creado por:** [gpradinett](https://github.com/gpradinett)

## Descripción

ZZZIPCRACK es un script en Bash que permite realizar ataques de diccionario a archivos ZIP protegidos con contraseña. Utiliza un diccionario de contraseñas y prueba cada una hasta encontrar la correcta.

El script está diseñado para ejecutarse en diferentes entornos de terminal, incluyendo soporte específico para Termux en Android, así como en sistemas Linux y Windows con Bash.

archive.zip : Ruta al archivo ZIP protegido con contraseña.
Dictionary.txt : Archivo de texto que contiene una lista de contraseñas para probar (una por línea).

## Uso

### Sintaxis

```bash
bash main.sh archive.zip dictionary.txt
```

### Requisitos
Linux/Windows : Tener instalado unzip. Puedes instalarlo usando tu gestor de paquetes:

En Ubuntu/Debian :
```bash
sudo apt-get install unzip
```
En Fedora 
```bash
sudo dnf install unzip
```
Termux :
```bash
pkg install unzip
```

Caracteristicas
Soporte de color en la terminal para una mejor visualización.
Mensajes de progreso y notificación al encontrar la contraseña.
Detecta y adapta el banner según el entorno de ejecución (Linux, Termux o Windows).
Detalles del Código
Verifique la existencia de los archivos de entrada antes de comenzar el ataque.
Realice un bucle para probar cada contraseña del diccionario.
Si encuentra la contraseña correcta, la muestra y termina la ejecución.
Muestra un mensaje de error si no se encuentra la contraseña.
Colores de la terminal
Azul : Indicadores de progreso.
Verde : Mensajes informativos.
Rojo : Mensajes de error o advertencia.

Asegúrese de que el script tenga permisos de ejecución:

```bash
chmod +x main.sh
```

Licencia
Este proyecto se distribuye bajo la licencia MIT.

Contacto
Para obtener más información o mejoras, comuníquese con gpradinett .


Puedes copiar y pegar este contenido directamente en tu archivo `README.md` en GitHub. ¡Si necesitas algo más, solo dímelo!


