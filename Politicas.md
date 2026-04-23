# Políticas de Zero Spam

**Última actualización:** abril de 2026  

**Aplicación:** Zero Spam (identificador de paquete: `com.zeroteam.zerospamapp`)  

**Editor responsable:** Zero Team (sustituye por la razón social o nombre comercial definitivo).

Este documento incluye la **Política de privacidad** y los **Términos de uso** de la aplicación móvil Zero Spam. Debes publicarlo en una **URL accesible públicamente** (sin contraseña) y enlazarlo en Google Play Console y, si aplica, en la propia app.

---

## Parte I — Política de privacidad

### 1. Introducción

Zero Spam es una aplicación para **Android** orientada a ayudar a los usuarios a **reducir llamadas y mensajes no deseados**, gestionar listas de permitidos/bloqueados, consultar información asociada a números de teléfono y, cuando el usuario lo decide, **enviar reportes** al servicio en la nube.

Al instalar o usar Zero Spam, aceptas el tratamiento de datos descrito en esta política, en la medida en que resulte aplicable a tu uso de la app.

### 2. Responsable del tratamiento

El responsable del tratamiento de los datos personales obtenidos a través de la app es el titular/editor indicado al inicio de este documento.  

**Contacto para ejercer derechos o consultas de privacidad:** sustituye por un correo electrónico o formulario de contacto válido (por ejemplo: `privacidad@tudominio.com`).

### 3. Datos que puede tratar la aplicación

Según las funciones que actives y los permisos que concedas, Zero Spam puede tratar, entre otros, los siguientes datos:

| Categoría | Ejemplos | Finalidad principal |
|-----------|----------|---------------------|
| **Identificadores de cuenta** | Correo electrónico, nombre para mostrar, identificador de usuario en el backend | Crear y mantener tu cuenta, iniciar sesión y sincronizar preferencias asociadas a la cuenta. |
| **Teléfono y verificación** | Número en formato internacional (E.164), estado de verificación del teléfono | Asociar la cuenta a un número, verificación por SMS/código y cumplir requisitos de rutas protegidas del servidor (p. ej. reportes o filtros avanzados). |
| **Datos de llamadas y SMS** | Número de origen/destino, metadatos necesarios para filtrado o pantalla de llamada, historial según permisos del sistema | Mostrar interfaz de llamada, evaluar si una llamada o mensaje es sospechoso, aplicar listas locales y sincronización con el servicio cuando corresponda. |
| **Contactos** | Datos de la agenda que el sistema permita leer o modificar con tu permiso | Integración con marcador, contactos y funciones que elijas usar. |
| **Datos técnicos y de uso** | Identificadores de publicidad, datos agregados de uso de la app, diagnósticos si los activas | Mejorar el producto, mostrar anuncios (ver sección de publicidad) y estabilidad. |
| **Tokens de sesión** | Tokens de acceso y renovación de sesión | Mantener la sesión iniciada de forma segura y llamar a APIs autenticadas. |

No solicitamos datos innecesarios para la categoría de la app; los permisos sensibles se usan en el marco de las funciones de **telefonía, SMS, contactos y protección frente a spam**.

### 4. Permisos del dispositivo (Android)

La app puede solicitar permisos declarados en el manifiesto, entre ellos (según versión del sistema y flujo de la app):

- **Teléfono y llamadas:** lectura de estado básico del teléfono, números asociados a la SIM cuando el sistema lo permita, registro de llamadas según política del fabricante, contestar o gestionar llamadas en el contexto de la app como cliente de llamadas.
- **SMS/MMS:** leer, enviar y recibir SMS/MMS cuando configures Zero Spam como app predeterminada o concedas los permisos correspondientes.
- **Contactos:** leer y escribir contactos si activas funciones que lo requieran.
- **Internet:** comunicación con servidores y servicios de terceros (autenticación, API, anuncios).
- **Notificaciones y primer plano:** mostrar avisos y mantener servicios de llamada cuando el sistema lo exija.

Puedes **revocar permisos** desde Ajustes de Android; algunas funciones dejarán de estar disponibles sin ellos.

### 5. Servicios de terceros y transferencias

#### 5.1 Backend propio (API)

La app se comunica con un **servidor backend** alojado en infraestructura en la nube (p. ej. Railway u otro proveedor equivalente) en la URL de producción configurada en la compilación, por ejemplo:

`https://zerospambackend-production.up.railway.app`

A través de ese servicio se pueden enviar o recibir, entre otros: datos de registro e inicio de sesión, listas de números permitidos/bloqueados, consultas sobre números, filtros tipo *bloom filter*, reportes de spam/incidentes y datos de suscripción/plan según la API documentada del proyecto.

El tratamiento en servidor debe ajustarse a lo que el **operador del backend** (Zero Team o quien ostente la titularidad) defina en sus propias bases legales y acuerdos con proveedores de hosting.

#### 5.2 Google (Firebase / inicio de sesión con Google)

Si usas **inicio de sesión con Google**, intervienen los servicios de Google según sus políticas. Google actúa como responsable o encargado según el caso respecto a los datos que trate directamente. Te recomendamos revisar la política de privacidad de Google.

#### 5.3 Publicidad (Google AdMob)

La app puede mostrar **anuncios** mediante el SDK de **Google AdMob**. Google puede usar identificadores de publicidad y datos técnicos conforme a su política de anuncios y privacidad. Puedes limitar la personalización de anuncios desde la configuración del sistema Android y, cuando esté disponible, desde las opciones de la app o del formulario de consentimiento aplicable en tu región.

### 6. Almacenamiento local y seguridad

- Parte de la información (listas, caché, preferencias, datos de sesión cifrados cuando aplique) puede guardarse **en el dispositivo**.
- Los **tokens de sesión** se gestionan con mecanismos de almacenamiento seguro del sistema (p. ej. preferencias cifradas respaldadas por el almacén de claves del dispositivo), según la implementación actual del proyecto.
- Debes **proteger el dispositivo** con bloqueo de pantalla y no compartir tu cuenta con terceros.

### 7. Conservación y supresión

- Los datos en el **dispositivo** permanecen hasta que desinstales la app o borres datos de la aplicación desde Ajustes de Android.
- Los datos en el **servidor** se conservan el tiempo necesario para prestar el servicio y cumplir obligaciones legales. Para solicitar **acceso, rectificación, supresión u oposición** (según la ley que te aplique, p. ej. GDPR en la UE o LFPDPPP en México), contacta al responsable en la dirección indicada en la sección 2.

Cerrar sesión o usar la función de **cierre de sesión / logout** en la app puede revocar tokens en el servidor según el diseño de la API (p. ej. invalidación del *refresh token*).

### 8. Menores de edad

Zero Spam **no está dirigida** a menores de 16 años (o la edad mínima que marque la ley de tu país). Si eres padre/madre o tutor y crees que un menor ha facilitado datos, contacta al responsable para solicitar su eliminación.

### 9. Cambios en esta política

Podemos actualizar esta política para reflejar cambios legales o en la app. La **fecha de actualización** figurará al inicio del documento. El uso continuado de la app tras publicar cambios puede implicar la aceptación de la versión revisada, salvo que la ley exija consentimiento adicional.

### 10. Ley aplicable y reclamaciones

Sustituye este apartado por la ley y tribunales que correspondan a tu entidad (por ejemplo, legislación mexicana o española) y, si aplica, el derecho a reclamar ante la **autoridad de protección de datos** de tu país.

---

## Parte II — Términos de uso

### 1. Objeto

Los presentes Términos regulan el uso de la aplicación **Zero Spam** para Android. Al descargar, instalar o usar la app, declaras que has leído y aceptas estos términos y la Política de privacidad.

Si **no estás de acuerdo**, no uses la aplicación.

### 2. Licencia de uso

Se te concede una licencia **personal, no exclusiva, revocable e intransferible** para usar Zero Spam conforme a lo permitido en Google Play y en este documento. No está permitido:

- Descompilar, hacer ingeniería inversa o eludir medidas de seguridad salvo lo permitido por ley imperativa.
- Usar la app para fines ilegales, acosar a terceros, enviar reportes falsos de forma sistemática o interferir con redes o servicios ajenos.
- Revender, alquilar o sublicenciar la app sin autorización escrita del titular.

### 3. Funcionalidad y aviso legal

- Zero Spam es una **herramienta de asistencia**; no garantiza bloquear el 100 % de llamadas o mensajes no deseados (depende de red, fabricante, permisos y listas).
- Las **valoraciones de riesgo** o etiquetas mostradas son orientativas y pueden basarse en datos locales, servidor o ambos.
- El usuario es **responsable** del uso que haga de la app (incluidos bloqueos, reportes y comunicaciones con terceros).

### 4. Cuenta y credenciales

Eres responsable de mantener la **confidencialidad** de tu contraseña y de las sesiones abiertas en tu dispositivo. Notifica de inmediato cualquier uso no autorizado si el titular del servicio ofrece un canal para ello.

### 5. Contenido y reportes

Si la app permite **reportar números** o incidentes:

- Debes aportar información **veraz** en la medida de tus conocimientos.
- No está permitido usar el sistema de reportes para fines difamatorios, discriminatorios o ilegales.

El titular del backend puede **moderar, rechazar o eliminar** contenidos o cuentas que incumplan la ley o estos términos.

### 6. Publicidad y versión gratuita

La versión distribuida puede incluir **publicidad** de terceros. Los anuncios son responsabilidad en parte de los anunciantes y de la red publicitaria; consulta la Política de privacidad para más detalle.

### 7. Modificaciones del servicio

El titular puede **actualizar, suspender o discontinuar** funciones o la app con el aviso que exija la ley o las políticas de la tienda de aplicaciones. No se garantiza mantenimiento indefinido de ninguna función concreta.

### 8. Limitación de responsabilidad

En la medida máxima permitida por la ley aplicable:

- El servicio se ofrece **“tal cual”** y según disponibilidad.
- No nos hacemos responsables de daños indirectos, lucro cesante, pérdida de datos o perjuicios derivados del uso o imposibilidad de uso de la app, salvo que la ley imperativa disponga lo contrario.

### 9. Legislación y resolución de conflictos

Sustituye por la **legislación y jurisdicción** que corresponda al titular del servicio (por ejemplo, tribunales de Ciudad de México o de Madrid). Si la ley de tu país como consumidor impone un fuero imperativo, prevalecerá dicho fuero.

### 10. Contacto

Para consultas sobre estos términos o la privacidad, utiliza el mismo contacto indicado en la **Parte I, sección 2** (sustituye el marcador de posición por datos reales antes de publicar).

---

**Nota para el equipo:** antes de publicar en Play Store, reemplaza los textos “sustituye por…”, el correo de contacto y la legislación aplicable. Opcionalmente añade un enlace a `Politicas.md` hospedado en tu sitio web o repositorio público estable.
