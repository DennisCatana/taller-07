# taller-07

## Repaso Final de JS<br>
![image](https://github.com/DennisCatana/taller-07/assets/150082943/2d8fc6da-d186-4b19-bd1e-179aad395c45)
![image](https://github.com/DennisCatana/taller-07/assets/150082943/f4705267-a908-49c5-9dcf-ba48d08fab07)

## Modelo cliente Servidor<br>
**Flujo Básico:**

1. **Solicitud del Cliente:**
   - El navegador envía solicitudes HTTP al servidor mediante acciones del usuario (clic en enlaces, envío de formularios).
   - La solicitud incluye detalles como la URL, método (GET, POST), y datos adicionales.

2. **Procesamiento en el Servidor:**
   - El servidor procesa la solicitud, determina la acción requerida y puede interactuar con bases de datos.
   
3. **Respuesta del Servidor:**
   - El servidor responde con un código de estado y el contenido solicitado (páginas HTML, datos).
   
4. **Representación en el Cliente:**
   - El navegador interpreta la respuesta y muestra la interfaz de usuario.
   - Puede realizar solicitudes adicionales para obtener recursos (CSS, JavaScript).

**Ciclo Continuo:**

- El flujo cliente-servidor se repite para cada interacción, permitiendo aplicaciones web dinámicas.

![image](https://github.com/DennisCatana/taller-07/assets/150082943/f3818687-55e1-4953-84c3-36382220c3bf)

## Servidor web con el módulo de Node.js HTTP<br>
*SERVIDOR HTTP* <br> 
![WhatsApp Image 2023-12-02 at 22 28 59](https://github.com/DennisCatana/taller-07/assets/117743538/99d68c2c-c253-44b5-a1c6-10c8d8c8f784) <br>

![WhatsApp Image 2023-12-02 at 22 33 11](https://github.com/DennisCatana/taller-07/assets/117743538/d3644958-bed3-4093-bc9e-71d019b01588) <br>

## Servidor web con el paquete de NPM Express<br>
![WhatsApp Image 2023-12-02 at 22 56 10](https://github.com/DennisCatana/taller-07/assets/117743538/a0152cdd-19cb-4371-8dd3-14ab820f66a4) <br>
![WhatsApp Image 2023-12-02 at 22 56 58](https://github.com/DennisCatana/taller-07/assets/117743538/43aeba99-6615-4e98-b60e-f4cc10f8cc42) <br>


## Estructura de directorios y carpetas para los futuros proyectos<br>
 
_Esta estructura es modulable y escalable que permite que diferentes partes de la app este organizada de manera mas clara._ <br>
![WhatsApp Image 2023-12-03 at 14 33 48](https://github.com/DennisCatana/taller-07/assets/117743538/d1118393-a53b-4c47-b526-57a314cb9eaa) <br>

## Realizar la consulta de cómo hacer el despliegue de un backend a un ambiente de producción (RAILWAY)

![RAILWAY](https://github.com/DennisCatana/taller-07/assets/117743120/bc5154d0-7646-441e-beae-d390c9cec4bf)

1. Registro en Railway:
Accede al sitio web de Railway y regístrate para obtener una cuenta.

2. Instalación de Railway CLI:
Abre tu terminal y sigue las instrucciones en la documentación de Railway para instalar la CLI. Esto te permitirá interactuar con Railway desde la línea de comandos.

3. Configuración del Proyecto:
Asegúrate de que tu proyecto tenga un archivo package.json para proyectos Node.js o el equivalente para otros lenguajes.

Añade un archivo railway.yml en la raíz de tu proyecto para configurar tu base de datos y otras variables de entorno.
Ejemplo de railway.yml para una aplicación Node.js con una base de datos PostgreSQL
services:
    name: backend<br>
    type: node<br>
    env:<br>
      DATABASE_URL: ${{DATABASE_URL}}<br>
databases:<br>
    name: postgres<br>
    type: postgresql

4. Variables de Entorno:
Configura las variables de entorno necesarias en el archivo railway.yml.

5. Despliegue:
Ejecuta el siguiente comando en tu terminal para desplegar tu aplicación: "railway run npm start"

