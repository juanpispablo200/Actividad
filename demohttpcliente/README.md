    Importación de paquetes: El código importa dos paquetes importantes para este ejemplo: flutter/material.dart para los componentes de Flutter y http/http.dart para realizar solicitudes HTTP.

    Función main(): La función main() es el punto de entrada de la aplicación Flutter. En este caso, simplemente ejecuta la función runApp() pasando una instancia de MyApp.

    Clase MyApp: Esta clase define la aplicación en sí misma. Es un widget de estado estático que devuelve una instancia de MaterialApp, que proporciona las funcionalidades básicas de una aplicación de Flutter.

    Clase MyHomePage: Esta clase define la página principal de la aplicación. Es un widget de estado que devuelve una instancia de Scaffold, que proporciona una estructura básica para la página.

    Método initState(): Este método se llama automáticamente cuando el widget es insertado en el árbol de widgets por primera vez. Aquí se llama _fetchPosts() para cargar los datos.

    Método _fetchPosts(): Este método utiliza el paquete http para realizar una solicitud GET a la URL https://jsonplaceholder.typicode.com/posts. Si la solicitud es exitosa (código de estado 200), decodifica la respuesta JSON y actualiza el estado de posts con los datos obtenidos. Si hay un error, lanza una excepción.

    Método build(): Este método construye la interfaz de usuario de la página principal. Devuelve un Scaffold con un AppBar que muestra el título de la aplicación y un ListView.builder que muestra una lista de publicaciones. Cada publicación se muestra como un ListTile con el título obtenido del campo 'title' de la respuesta JSON.![Captura de pantalla 2024-02-10 110403](https://github.com/juanpispablo200/Actividad/assets/116582110/71b03afe-8552-4a5e-ae14-b8a8c4cf744a)
