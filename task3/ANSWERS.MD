1. What does the `visible` prop of `Modal` do and why do we control it with `useState`?
R: Visible se usa para mostrar el modal; con useState se puede ocultar al usuario o volver a mostrarlo
2. What is `onRequestClose` for? What happens on Android if you do not close the modal in it?
R: Sirve para responder a una solicitud de cierre del sistema en Android, por ejemplo, cuando el usuario presiona el botón Atrás. Si no gestionamos ese evento para cerrar el modal, el botón Atrás no podrá cerrarlo como se espera
3. What is the effect of `transparent={true}`? Name the three values of `animationType`.
R:transparent={true} Hace posible la transparencia en un modal y los 3 valores son: slide, fade, none
4. Why does `ScrollView` exist? What happens with a long `View` without it? When would you choose `FlatList` instead?
R:ScrollView permite desplazarse para ver contenido en la pantalla; con los views no es posible hacer desplazamiento; los elementos quedarían fuera de pantalla, mientras que los FlatList renderizan los elementos a medida que se necesitan
5. What is the difference between the `style` and the `contentContainerStyle` props of a `ScrollView`?
R: El estilo se aplica al mismo contenedor exterior, mientras que el otro se aplica al contenedor interior
6. What is `SafeAreaView` for and which zones of the device does it protect? Why do we use `react-native-safe-area-context`?
R:Es para que el contenido no quede tapado por elementos del dispositivo o sistema, como la cámara o notch, la barra de estado y la zona de navegación inferior. Se recomienda usar react-native-safe-area-context para gestionar de manera más flexible las áreas seguras
7. Write the three best practices from the Step 5 checklist in your own words and give an example of when a modal is **not** a good idea.
Usar un solo modal en la pantalla y reservarlo para una acción breve y específica.
R1:Limitar el contenido de los ScrollView; en esta tarea, las listas 
R2:largas son PROJECTS (5 elementos) y CONTACTS (8 elementos).
R3:Colocar la pantalla dentro de SafeAreaView.
R4:Un modal no suele ser buena opción para un mensaje informativo pequeño, como “Cambios guardados”. Es mejor mostrarlo dentro de la pantalla, por ejemplo como un mensaje breve, porque un modal interrumpe lo que la persona estaba haciendo.