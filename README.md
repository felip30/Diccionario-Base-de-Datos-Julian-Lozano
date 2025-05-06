# Diccionario-Base-de-Datos-Julian-Lozano
# 📂 Diccionario de Base de Datos - ConfisoftW

## 📜 Descripción
Este diccionario de base de datos documenta las estructuras y tipos de datos utilizados en la aplicación **ConfisoftW**. Contiene información detallada sobre entidades clave como **usuarios, facturas, clientes, reportes, productos y pedidos**.

## 🛠 Estructura de la Base de Datos
El diccionario de datos se organiza en distintas entidades, cada una con sus respectivos campos, tipos de datos y descripciones:

### 🧑‍💻 **Usuarios**
| Campo         | Tipo de Dato | Tamaño       | Descripción |
|--------------|-------------|-------------|-------------|
| `idUsuario`  | `INT`       | `4 BYTES`   | Identificador único del usuario |
| `tipoDocumento` | `VARCHAR` | `15 CARACTERES` | Tipo de documento (CC, TI, Pasaporte) |
| `documento` | `VARCHAR` | `20 CARACTERES` | Número de documento del usuario |
| `nombres` | `VARCHAR` | `50 CARACTERES` | Nombres completos |
| `apellidos` | `VARCHAR` | `50 CARACTERES` | Apellidos completos |
| `usuario` | `VARCHAR` | `20 CARACTERES` | Nombre de usuario para autenticación |
| `contraseña` | `VARCHAR` | `255 CARACTERES` | Contraseña cifrada |
| `email` | `VARCHAR` | `100 CARACTERES` | Correo electrónico |
| `telefono` | `VARCHAR` | `15 CARACTERES` | Teléfono de contacto |

### 🏷 **Facturas**
| Campo         | Tipo de Dato | Tamaño       | Descripción |
|--------------|-------------|-------------|-------------|
| `idFactura`  | `INT`       | `4 BYTES`   | Identificador único de la factura |
| `idPedido`  | `INT`       | `4 BYTES`   | Identificador del pedido asociado |
| `fechaFactura` | `DATE`    | `4 BYTES`   | Fecha de generación de la factura |
| `montoTotal` | `DECIMAL`  | `10,2 BYTES` | Total del monto facturado |
| `clienteNombre` | `VARCHAR` | `50 CARACTERES` | Nombre del cliente |
| `clienteEmail` | `VARCHAR` | `100 CARACTERES` | Correo electrónico asociado a la factura |
| `productosFacturados` | `TEXT` | `N/A` | Detalle de productos incluidos en la factura |


## 📑 Uso del Diccionario
- **Propósito**: Facilitar la consulta de estructuras de datos en el desarrollo de la aplicación.
- **Formato**: El archivo está estructurado en **Markdown** para una visualización clara en GitHub.
- **Modificaciones**: Cualquier actualización de la base de datos debe reflejarse en este documento.

## 📌 Notas
- Se recomienda mantener este diccionario **actualizado** para evitar discrepancias con la implementación real.
- Utilizar nombres de campos **coherentes** con la lógica del sistema.
- Validar restricciones y relaciones entre entidades para asegurar la integridad de los datos.

