# GPS Map ML

## Descripción del Proyecto
GPS Map ML es una aplicación Android que utiliza la API de Google Maps para mostrar la ubicación actual del usuario en un mapa. La aplicación permite visualizar la ubicación exacta, marcándola con un marcador personalizado, y brinda una interfaz simple para obtener y visualizar información de ubicación en tiempo real.

## Características
- Visualización en tiempo real de la ubicación del usuario utilizando Google Maps.
- Actualización automática de la ubicación al abrir la aplicación.
- Marcador en el mapa que indica la ubicación actual del usuario.
- Gestión de permisos de ubicación en tiempo de ejecución.
- Manejo de errores si no se puede obtener la ubicación del usuario.

## Requisitos
- **API de Google Maps**: Se debe configurar una clave API en la consola de Google Cloud.
- **Android 6.0 (API nivel 23)** o superior.
- **Permisos de ubicación**: La aplicación solicita permisos de ubicación precisa (ACCESS_FINE_LOCATION).

## Instalación
1. Clona este repositorio:
    ```bash
    git clone https://github.com/Ferna-n/GPSMapML.git
    ```
2. Abre el proyecto en Android Studio.
3. Agrega la clave API de Google Maps en el archivo `AndroidManifest.xml`:
    ```xml
    <meta-data
        android:name="com.google.android.geo.API_KEY"
        android:value="TU_API_KEY"/>
    ```
4. Ejecuta la aplicación en un emulador o dispositivo físico con Android.

## Uso
1. Al abrir la aplicación, se solicitarán permisos de ubicación. Concede los permisos para que la aplicación pueda obtener tu ubicación actual.
2. Una vez concedidos los permisos, el mapa mostrará tu ubicación con un marcador.
3. Si la ubicación no está disponible, la aplicación te notificará con un mensaje de error.

## Estructura del Proyecto
- **MainActivity.java**: Contiene la lógica principal de la aplicación, incluyendo la gestión de permisos y la integración con Google Maps.
- **activity_main.xml**: Archivo de layout que define la interfaz de usuario y el fragmento del mapa.
- **AndroidManifest.xml**: Define los permisos necesarios y la configuración de la clave API de Google Maps.

## Licencia
Este proyecto está bajo la licencia MIT - ver el archivo [LICENSE](LICENSE) para más detalles.
