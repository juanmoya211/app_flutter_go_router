📱 **Flutter GoRouter y pantallas básicas**
 
📝 **Descripción**
 
🌐 Esta es una aplicación móvil desarrollada en Flutter, diseñada para demostrar la navegación entre pantallas usando la librería GoRouter. La app permite moverse de forma sencilla entre una pantalla principal y una segunda pantalla, facilitando la comprensión del enrutamiento en Flutter.
 
❗ **Problema**
 
Toda aplicación con varias pantallas necesita un sistema de navegación claro. Sin usar un enrutador estructurado, cambiar de pantalla puede volverse confuso y difícil de mantener a medida que crece el proyecto.
 
💡 **Solución**
 
Usamos GoRouter, la librería oficial recomendada para gestionar las rutas en Flutter. Con GoRouter definimos cada pantalla como una ruta, y desde cualquier botón podemos llamar esa ruta para navegar.
 
📦 **Cómo Ejecutar**
 
**Prerrequisitos**
 
- ✅ Flutter SDK instalado

- ✅ GoRouter agregado en  pubspec.yaml 
 
🚀 **Instalación y Ejecución**
 
1. Abre el proyecto en Visual Studio Code

2. Abre la terminal y ejecuta:

```dart
flutter pub get
```

```dart
flutter run
```

Cuando te pregunte el dispositivo, elige la opción de Chrome para ejecutarla en el navegador.
 
🧾 **Explicación del código principal**
 
 **GoRouter :** Es el objeto que guarda todas tus rutas.
 
```dart
final GoRouter _router = GoRouter(
  routes: [
    GoRoute(
      path: '/',
      builder: (context, state) => const HomeScreen(),
    ),
    GoRoute(
      path: '/segunda',
      builder: (context, state) => const SegundaPantalla(),
    ),
  ],
);
```

-  ```dart path: '/' ``` → es la pantalla principal, la ruta por defecto
​
-  ```dart path: '/segunda' ```  → es la ruta de la segunda pantalla
 
**Navegar con el botón:**

```dart onPressed: () => context.go('/segunda'), ```

Con  ```dart context.go('ruta') ``` le decimos a GoRouter que nos lleve a esa pantalla.
 
**📸 Evidencias**
 
**Pantalla Principal**
 
<img width="1366" height="718" alt="pantalla principal" src="https://github.com/user-attachments/assets/0ab8d7fc-693b-480a-8e1c-a5ef4c11c1ce" />



 
**Segunda Pantalla**
 
<img width="1366" height="711" alt="segunda pantalla" src="https://github.com/user-attachments/assets/3c393c17-9cab-4767-a35c-9266d8b96f09" />


👤 **Autor**

Juan David Moya Corrales

Curso: Optativa I

Código del curso: 650202015 -1
