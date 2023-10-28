<p align="center">
  <img src="https://github.com/CaMiLoTuTa/IgualApp/blob/main/img/iconos/bannerNegroA.png?raw=true" alt="IgualApp Logo" width="400"/>
</p>

<h6 align="right">Adrián Camilo Tuta Cortés, Miguel Ángel Bejarano e Irving Rios Ramirez.</h6>
<h6 align="right">27 de octubre de 2023</h6>

---

<h2 align="center">Juntos, Sin Barreras.</h2>

- <u>**Problemática**</u>

  - Financia proyectos de infraestructura básica.

---

<h2 align="center">Descripción del Proyecto</h2>

 <h6 align="center">Juntos, Sin Barreras</h6>
<u>**IgualApp** es una aplicación diseñada para abordar el racismo y la discriminación al promover la igualdad y la diversidad en la sociedad</u>. La aplicación utiliza la tecnología para crear conciencia y fomentar el cambio social. Ofrece recursos educativos y promueve la interacción comunitaria para empoderar a los usuarios y combatir el racismo. Además, incluye una función que permite a los usuarios registrar incidentes de racismo para recibir ayuda inmediata. El objetivo principal de IgualApp es brindar apoyo a personas que enfrentan racismo, promoviendo la igualdad y la inclusión a través de la educación y la acción comunitaria.

### 1. Evaluación de Ventajas y Desventajas:

| **Ventajas**                                | **Desventajas**               |
| ------------------------------------------- | ----------------------------- |
| Lucha contra el racismo y la discriminación | Complejidad de Implementación |
| Promoción de la igualdad y la diversidad    | Necesidad de Datos Precisos   |
| Sensibilización y cambio social             | Costo Inicial                 |
| Empoderamiento de usuarios                  | Limitaciones Tecnológicas     |
| Registro de incidentes para ayuda inmediata | Público objetivo              |

### 2. Definición General:

#### 2.1. _Definición del Problema:_

El problema abordado por este proyecto es la presencia persistente de racismo y discriminación en la sociedad. Estos problemas afectan a individuos y comunidades, causando daño emocional, social y a veces incluso físico. El racismo y la discriminación son barreras para la igualdad y la diversidad, lo que hace que sea esencial abordarlos de manera efectiva.

#### 2.2. _Solución Ofrecida:_

La solución ofrecida es "IgualApp", una aplicación diseñada para combatir el racismo y la discriminación. La aplicación busca promover la igualdad y la diversidad a través de recursos educativos, interacción comunitaria y la capacidad de registrar incidentes de racismo para obtener ayuda inmediata. Además, la aplicación fomenta la conciencia y el cambio social, empoderando a los usuarios para tomar medidas contra la discriminación.

#### 2.3. _Justificación:_

Este proyecto radica en la necesidad de abordar un problema social significativo y perjudicial, como el racismo y la discriminación. Estos problemas persisten en muchas partes del mundo y tienen un impacto negativo en la vida de las personas. La igualdad y la diversidad son valores fundamentales para una sociedad justa, y esta aplicación busca promover esos valores y crear un mundo más inclusivo.

#### 2.4. _Usuario Final:_

Serán todas las personas que deseen contribuir a la lucha contra el racismo y la discriminación. Esto incluye a personas que han experimentado el racismo, así como a aquellos que desean aprender más sobre el tema y tomar medidas para combatirlo. La aplicación está diseñada para ser accesible para personas de todas las edades y antecedentes.

#### 2.5. _Utilidad:_

Capacidad para proporcionar recursos educativos, fomentar la interacción comunitaria, registrar incidentes de racismo y brindar ayuda inmediata. La aplicación empodera a los usuarios al permitirles aprender, compartir experiencias y solicitar asistencia en situaciones de discriminación. Su utilidad se extiende a la promoción de la igualdad y la diversidad en la sociedad y a la creación de una red de apoyo para aquellos que enfrentan problemas de racismo.

#### 2.6. _Espacio de Trabajo:_

Toda la documentación relacionada con el proyecto se almacenará en la página del proyecto en **GitHub**. Esto facilitará la colaboración entre los miembros del equipo y el acceso a la información relevante.

## 3. ESPECIFICACIÓN INICIAL DE REQUERIMIENTOS:

### 3.1. _Requerimientos Funcionales:_

- Si el campo de correo o contraseña no están llenos, el botón de ingreso se bloqueará. El campo de **correo debe contener al menos 11 caracteres** y la **contraseña al menos 8** caracteres para habilitar el botón.
- Se debe mostrar un **mensaje de error** si las credenciales ingresadas en la pantalla de inicio de sesión no son correctas.
- En caso de **falta de conexión** a internet, se mostrará un mensaje de **advertencia**.
- **Los cambios** realizados por un administrador **se registrarán**, mostrando quién realizó el cambio y la fecha en la pestaña correspondiente.
- La contraseña se mostrará como una serie de \* para proteger su visibilidad.

#### 3.1.1. Pantalla de Inicio de Sesión:

- Si el usuario no ingresa correctamente el correo o la contraseña, se mostrará un mensaje de "Contraseña incorrecta".
- La base de datos se actualizará con la **fecha actual** cuando un usuario inicie sesión.
- Los usuarios **tendrán tres intentos** para ingresar la contraseña correctamente. Después de tres intentos fallidos, se bloqueará el acceso y se enviará un correo de alerta.
- Si el usuario no se encuentra registrado, se redirigirá al usuario a la pestaña de registro.
- El botón de ingreso solo estará activo si el campo de correo contiene "@gmail.com" o "@outlook.com".
- Las credenciales ingresadas en la pantalla de inicio de sesión se guardarán y autocompletarán si el usuario vuelve a esta pantalla después de iniciar sesión.

#### 3.1.2. Pantalla de Registro:

- El botón "Enviar código de confirmación" se activará solo si el campo de correo contiene al menos 11 caracteres.
- Tras presionar el botón "Enviar código de confirmación", se generará y **enviará un código aleatorio de 6 dígitos** por correo electrónico.
- Los usuarios tendrán cuatro intentos para ingresar correctamente el código de confirmación. Tras cuatro intentos fallidos, se bloqueará la pantalla de registro.
- Se requerirá la confirmación de **contraseña ingresada dos veces** para activar el botón de registro.
- Si todas las credenciales cumplen con los requisitos, se enviará un correo de bienvenida, se guardarán sus credenciales en la base de datos y se esperará la confirmación de su tipo de usuario.

#### 3.1.3. Pantalla de Recuperación de Contraseña:

- El botón "Enviar código de confirmación" se activará solo si el campo de correo contiene al menos 11 caracteres y **contiene explícitamente "@gmail.com" o "@outlook.com"**.
- Tras presionar el botón "Enviar código de confirmación", se generará y enviará un código aleatorio de 6 dígitos por correo electrónico.
- Los usuarios tendrán cuatro intentos para ingresar correctamente el código de confirmación. Tras cuatro intentos fallidos, se bloqueará la pantalla de recuperación de contraseña.
- Se requerirá la confirmación de contraseña ingresada dos veces para activar el botón de cambio de contraseña.

#### 3.1.4. Pantalla Principal:

- La pantalla principal ofrecerá una entrada clara a la aplicación, **presentando opciones** y funciones clave.
- Los usuarios podrán **acceder a todas las áreas** esenciales de la aplicación desde esta pantalla.
- La disposición de características **será organizada y coherente**, priorizando la usabilidad y evitando características complejas.

<!-- TODO: PONER PANTALLAS QUE SON Y MODIFICARLAS SEGÚN LA APLICACIÓN -->

#### 3.1.5. Pantalla de Modelado y Simulación:

#### 3.1.6. Pantalla de Informes y Gráficos:

#### 3.1.7. Pantalla de Configuración:

#### 3.1.8. Pantalla de Ayuda y Soporte:

- Se proporcionará **información completa** y accesible para ayudar a los usuarios.
- Los recursos de ayuda serán consistentes y precisos, ofreciendo soluciones para **problemas comunes**.
- La actualización y adición de recursos será posible según necesidades cambiantes.

#### 3.1.9. Pantalla de Administración de Usuarios:

- Los administradores podrán **gestionar usuarios** y roles de manera eficiente.
- Se brindarán funciones para agregar, modificar y eliminar usuarios, así como asignar roles; **CRUD**.
- La presentación será uniforme y las acciones de administración serán precisas.

#### 3.1.10. Pantalla de Notificaciones:

- Se proporcionarán notificaciones relevantes y **oportunas** a los usuarios.
- La presentación de notificaciones será coherente y permitirá la personalización.
- Se garantizará la **precisión de la información** enviada.

#### 3.1.11. Pantalla de Actualizaciones y Novedades:

### 3.2. _Requerimientos No Funcionales:_

#### 3.2.1. **Gráficas en Tiempo Real:**

#### 3.2.2. **Subida de Modelos de Procesos:**

#### 3.2.3. **Actualizaciones en Cada Lanzamiento:**

La aplicación hará un proceso de actualización en cada lanzamiento para garantizar la incorporación de nuevas características y correcciones. Los usuarios recibirán **notificaciones claras sobre las actualizaciones** y podrán acceder a detalles sobre los cambios realizados.

#### 3.2.4. **Gama de Colores Adecuados:**

La interfaz de la aplicación utilizará una gama de colores diseñada específicamente para el **contexto industrial** al que está dirigida. Se priorizará la elección de colores que sean legibles, contrastantes y adecuados para transmitir información de manera clara.

Mas información en el **apartado 3** de la aplicación.

#### 3.2.5. **Control de Edición en la Aplicación:**

#### 3.2.6. **Almacenamiento de Cuentas en la Base de Datos:**

Las cuentas de **usuarios almacenadas en la base de datos** se asegurarán mediante medidas de seguridad adecuadas, como el cifrado de contraseñas. Se implementará un proceso de **eliminación segura** para las cuentas que no hayan sido utilizadas en un período de tres meses.

#### 3.2.7. **Eliminación de Cuentas Inactivas:**

Las cuentas de usuarios que **no se utilicen durante más de tres meses serán identificadas como inactivas**. Antes de eliminarlas, **se notificará** a los usuarios sobre la posible eliminación y se proporcionará un período de tiempo para reactivar su cuenta si así lo desean.

#### 3.2.8. **Tipos de Usuario y sus Roles:**

Los usuarios de la aplicación "IgualApp" se dividirán en distintos tipos, cada uno con roles y permisos específicos:

- _Usuarios Registrados:_ Son los usuarios estándar de la aplicación que han creado una cuenta. Sus funciones principales incluyen:

  - Registrarse y crear un perfil.
  - Acceder a recursos educativos sobre igualdad y diversidad.
  - Participar en comunidades y foros de discusión.
  - Reportar incidentes de racismo y discriminación.

- _Moderadores de Contenido:_ Estos usuarios tienen la responsabilidad de supervisar y gestionar el contenido de la aplicación. Sus funciones incluyen:

  - Revisar y aprobar publicaciones en los foros y comunidades.
  - Eliminar contenido inapropiado o ofensivo.
  - Ayudar a mantener un entorno seguro y respetuoso en la aplicación.

- _Administradores de la Comunidad:_ Los administradores de la comunidad tienen un rol más amplio en la gestión de las interacciones entre usuarios. Sus funciones abarcan:

  - Mediar en conflictos y debates en la comunidad.
  - Fomentar la participación activa y el respeto mutuo.
  - Reportar problemas graves a los moderadores o administradores superiores.

- _Administradores de la Aplicación:_ Estos administradores tienen un acceso más amplio y poderes de gestión de la aplicación. Sus funciones principales incluyen:

  - Administrar usuarios, roles y permisos.
  - Supervisar el registro de incidentes y proporcionar asistencia en situaciones críticas.
  - Realizar mantenimiento técnico y actualizaciones de la aplicación.

- _Administradores Superiores:_ Los administradores superiores son responsables de la gestión global de la aplicación y de la toma de decisiones estratégicas. Sus funciones abarcan:
  - Definir políticas y directrices de la aplicación.
  - Tomar decisiones importantes sobre el funcionamiento y el enfoque de "IgualApp".
  - Resolver problemas y conflictos a nivel de alto impacto.

Estos roles permiten una gestión eficaz y segura de "IgualApp" y garantizan que diferentes aspectos de la aplicación sean atendidos por personal especializado. Ten en cuenta que estos roles son una propuesta y pueden ajustarse según las necesidades específicas de tu aplicación y comunidad.

#### 3.2.10. **Seguridad y Privacidad:**

Se implementarán medidas de seguridad sólidas para proteger la información de los usuarios y garantizar la confidencialidad de los datos almacenados en la aplicación. Esto incluirá el **cifrado de datos sensibles y la autenticación segura**.

#### 3.2.11. **Escalabilidad:**

La aplicación estará diseñada para ser escalable y capaz de manejar un **aumento en la cantidad de datos e información**. Se optimizará **el rendimiento** y la capacidad de respuesta para asegurar una experiencia fluida incluso en momentos de alta demanda.

#### 3.2.12. **Compatibilidad:**

La aplicación estará diseñada para ser compatible con sistemas operativos como: Android, IOS.

### 3.3. Alcances del sistema:

- Se implementarán las funcionalidades esenciales definidas en los **Requerimientos Funcionales y No Funcionales**.
- Se priorizará la **funcionalidad** sobre la estética en la interfaz de usuario.
- El sistema se desarrollará de manera iterativa, con actualizaciones basadas en retroalimentación.

### 3.4. Tecnologías seleccionadas:

- _Lenguaje de Programación_: **JavaScript**.
- _Entorno de Desarrollo_: Visual Studio Code, **NeoVim**.
- _Bibliotecas y Frameworks_: **React Native**, Redux, Axios, Fetch
  Styled-components, Emotion, React Bootstrap, Material-UI, Formik,React Hook Form, React Query, SWR, React Helmet.
- _Base de Datos_: **MySQL**.
- _Control de Versiones_: Git.
- _Plataforma de Despliegue_: Docker.

---

# <center> <h6>APLICACIÓN</h6></center>

<!-- LOGO: [Looka](https://looka.com/dashboard) -->

### 1. LOGOS

- #### Icono de la aplicación:

  <p align="center">
    <img src="https://github.com/CaMiLoTuTa/IgualApp/blob/main/img/iconos/iconA.png?raw=true" alt="IgualApp icon" width="200"/>
  </p>

- #### Logo grande:

  <p align="center">
    <img src="https://github.com/CaMiLoTuTa/IgualApp/blob/main/img/iconos/bannerNegroA.png?raw=true" alt="IgualApp banner" width="300"/>
  </p>

### 2. TIPOGRAFÍA

- Títulos: **_MOON GET_**.
- Textos o información: Nunito, Montserrat, Lato.
- Botones: Source Sans Pro, FSP DEMO - Proxima Nova.

### 3. COLORES

<!-- https://www.happyhues.co/palettes/4 -->

| Elemento       | Código de Color | Ejemplo                                                                                                                                           |
| -------------- | --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| Fondo          | `#16161a`       | <img src="https://github.com/CaMiLoTuTa/IgualApp/blob/main/img/colores/colorFondo.png?raw=true" alt="Color de Fondo " width="200"/>               |
| Encabezado     | `#fffffe`       | <img src="https://github.com/CaMiLoTuTa/IgualApp/blob/main/img/colores/colorEncabezado.png?raw=true" alt="Color de Encabezado " width="200"/>     |
| Párrafo        | `#94a1b2`       | <img src="https://github.com/CaMiLoTuTa/IgualApp/blob/main/img/colores/colorParrafo.png?raw=true" alt="Color de Párrafo " width="200"/>           |
| Botón          | `#7f5af0`       | <img src="https://github.com/CaMiLoTuTa/IgualApp/blob/main/img/colores/colorBoton.png?raw=true" alt="Color de Botón " width="200"/>               |
| Texto de Botón | `#fffffe`       | <img src="https://github.com/CaMiLoTuTa/IgualApp/blob/main/img/colores/colorTextoBoton.png?raw=true" alt="Color de Texto de Botón " width="200"/> |
| Resaltado      | `#7f5af0`       | <img src="https://github.com/CaMiLoTuTa/IgualApp/blob/main/img/colores/colorResaltado.png?raw=true" alt="Color de Resaltado " width="200"/>       |
| Borde          | `#010101`       | <img src="https://github.com/CaMiLoTuTa/IgualApp/blob/main/img/colores/colorBorde.png?raw=true" alt="Color de Borde " width="200"/>               |
| Principal      | `#fffffe`       | <img src="https://github.com/CaMiLoTuTa/IgualApp/blob/main/img/colores/colorPrincipal.png?raw=true" alt="Color de Principal " width="200"/>       |
| Secundario     | `#72757e`       | <img src="https://github.com/CaMiLoTuTa/IgualApp/blob/main/img/colores/colorSecundario.png?raw=true" alt="Color de Secundario " width="200"/>     |
| Terciario      | `#2cb67d`       | <img src="https://github.com/CaMiLoTuTa/IgualApp/blob/main/img/colores/colorTerciario.png?raw=true" alt="Color de Terciario " width="200"/>       |

### 3. PANTALLAS

- **Pantalla de Inicio de Sesión:**

  - Permite a los usuarios ingresar sus credenciales para acceder a la aplicación.

- **Pantalla de Registro:**

  - Permite a los nuevos usuarios crear una cuenta en la aplicación.

- **Pantalla Principal:**

  - Muestra una visión general de la aplicación, sus objetivos y su propósito en la lucha contra el racismo.

- **Pantalla de Recursos Educativos:**

  - Proporciona acceso a artículos, videos, libros y otros recursos educativos relacionados con la igualdad y la diversidad.

- **Pantalla de Comunidad:**

  - Permite a los usuarios participar en discusiones, compartir experiencias y colaborar en iniciativas de igualdad.

- **Pantalla de Denuncia de Incidentes:**

  - Ofrece a los usuarios la capacidad de reportar incidentes de racismo y discriminación, con la opción de registrar su ubicación y detalles.

- **Pantalla de Información y Estadísticas:**

  - Muestra estadísticas y datos relacionados con el racismo y la discriminación, así como historias de éxito y avances.

- **Pantalla de Perfil de Usuario:**

  - Permite a los usuarios gestionar su perfil, configurar notificaciones y ver su actividad en la aplicación.

- **Pantalla de Ayuda y Soporte:**

  - Proporciona información y recursos de ayuda para los usuarios que puedan tener preguntas o problemas relacionados con el racismo.

- **Pantalla de Notificaciones:**

  - Muestra notificaciones importantes, actualizaciones de contenido y eventos relacionados con la igualdad.

- **Pantalla de Configuración:**

  - Permite a los usuarios personalizar su experiencia, ajustar preferencias y configurar notificaciones.

- **Pantalla de Actualizaciones y Novedades:**
  - Informa a los usuarios sobre nuevos recursos, eventos y campañas relacionados con la igualdad y la lucha contra el racismo.

<!-- ### 5. Funcionalidades Destacadas: -->

<!-- [Listado de las funcionalidades clave de la aplicación GreenOps que la hacen destacar y diferenciarse de otras soluciones similares.] -->

<!-- ### 6. Requisitos del Sistema: -->

<!-- [Especificación de los requisitos mínimos del sistema para ejecutar la aplicación, como sistema operativo, versión de Java, memoria RAM, espacio de almacenamiento, etc.] -->

<!-- ### 7. Instalación: -->

<!-- [Instrucciones detalladas para instalar la aplicación en diferentes plataformas (Windows, macOS, Linux).] -->

<!-- ### 8. Guía de Uso: -->

<!-- [Guía paso a paso sobre cómo utilizar cada una de las pantallas mencionadas anteriormente, explicando las funcionalidades y opciones disponibles.] -->

<!-- ### 9. Contribución: -->

<!-- [Invitación a la comunidad de desarrolladores a contribuir al proyecto, proporcionando información sobre cómo realizar contribuciones y el proceso de solicitud de incorporación de cambios (pull requests).] -->

<!-- ### 10. Equipo de Desarrollo: -->

<!-- [Presentación del equipo de desarrollo responsable del proyecto, mencionando sus roles y responsabilidades.] -->

<!-- ### 11. Licencia: -->

<!-- [Especificación de la licencia bajo la cual se distribuye el código fuente de la aplicación GreenOps y aclaración de los términos y condiciones de uso.] -->

<!-- ### 12. Contacto y Soporte: -->

<!-- [Información de contacto para consultas, soporte técnico y cualquier otro tipo de comunicación relacionada con el proyecto.] -->

<!-- ### 13. Información Adicional: -->

<!-- [Inclusión de cualquier otro dato relevante o particular sobre la aplicación GreenOps que se desee resaltar.] -->
