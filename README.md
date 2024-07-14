# Conversor de Monedas - Proyecto en Java

## Descripción del Proyecto

El conversor de monedas es una aplicación de escritorio desarrollada en Java que permite a los usuarios convertir cantidades entre diferentes monedas utilizando una API para obtener tasas de cambio actualizadas. La aplicación tiene una interfaz gráfica de usuario (GUI) que facilita la interacción del usuario.

## Tecnologías Utilizadas

- **Java:** Lenguaje de programación principal utilizado para el desarrollo del proyecto.
- **Swing:** Biblioteca gráfica de Java utilizada para crear la interfaz gráfica de usuario.
- **API de Open Exchange Rates:** Servicio web utilizado para obtener las tasas de cambio de divisas actualizadas.
- **JSON:** Formato de intercambio de datos utilizado para procesar las respuestas de la API.
- **BigDecimal:** Clase de Java utilizada para manejar operaciones matemáticas de alta precisión.

## Estructura del Proyecto

El proyecto se divide en varios paquetes y clases:

- **Paquete controlador**
  - `Convertir.java`: Contiene métodos para convertir descripciones de moneda en símbolos correspondientes.
  - `MiUrl.java`: Contiene métodos para abrir URLs en el navegador predeterminado.

- **Paquete modelo**
  - `EventoDeCaracters.java`: Contiene métodos para restringir la entrada del usuario a caracteres permitidos (letras, números, decimales).

- **Paquete vista**
  - `Inicio.java`: Clase principal que define la interfaz gráfica de usuario y maneja la lógica de conversión de divisas.

## Funcionalidades

- **Conversión de Divisas:** Permite a los usuarios ingresar una cantidad en una moneda y convertirla a otra utilizando tasas de cambio actualizadas.
- **Validación de Entrada:** Restringe la entrada del usuario para permitir solo caracteres válidos (números y decimales).
- **Interfaz Gráfica:** Proporciona una GUI fácil de usar para seleccionar monedas y mostrar los resultados de la conversión.

## Instalación y Ejecución

### Requisitos Previos

- **Java Development Kit (JDK):** Asegúrese de tener instalado el JDK en su sistema. Puede descargarlo desde Oracle o OpenJDK.
- **IDE de Java:** Se recomienda utilizar un entorno de desarrollo integrado (IDE) como IntelliJ IDEA, Eclipse o NetBeans para facilitar el desarrollo y la ejecución del proyecto.

### Pasos de Instalación

1. **Clonar el Repositorio:**

   ```bash
   git clone [https://github.com/tu-usuario/conversor-de-monedas.git](https://github.com/IvanGt1/Divisas)
2. Importar el Proyecto en el IDE

1. **Abra su IDE de Java preferido.**
2. **Importe el proyecto clonado como un proyecto de Java existente.**

### Agregar Dependencias

- Asegúrese de tener las bibliotecas necesarias, como JSON, en el classpath del proyecto. Puede agregar la biblioteca JSON descargándola desde JSON.org y agregándola a las librerías del proyecto.

### Ejecutar la Aplicación

1. **Busque la clase `Inicio.java` en el paquete `vista`.**
2. **Ejecute la clase `Inicio` como una aplicación Java.**

### Uso de la Aplicación

1. **Abrir la Aplicación:**
   - Ejecute la clase `Inicio.java` para abrir la GUI de la aplicación.

2. **Ingresar la Cantidad:**
   - Ingrese la cantidad que desea convertir en el campo de texto.

3. **Seleccionar Monedas:**
   - Seleccione la moneda de origen y la moneda de destino de los menús desplegables.

4. **Convertir:**
   - Haga clic en el botón "Convertir" para realizar la conversión. El resultado se mostrará en el campo de texto de resultado.

### Configuración de la API

Para utilizar la API de Open Exchange Rates:

1. **Registro en Open Exchange Rates:**
   - Regístrese en Open Exchange Rates para obtener una clave de API (app_id).

2. **Configuración Automática de la Clave de API:**
   - El proyecto está configurado para cargar automáticamente la clave de API desde un archivo `config.properties` ubicado en el directorio raíz del proyecto.
   - Asegúrese de no incluir `config.properties` en su repositorio Git para mantener segura su clave de API.
