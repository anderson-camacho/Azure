# Resumen de los Conceptos de Datos Principales

## Introducción

En el mundo de la informática, el manejo de los datos es esencial para el desarrollo de sistemas y aplicaciones. Los datos se representan en diferentes formatos, estructuras y almacenamientos, y su correcta gestión es fundamental para la eficiencia de cualquier sistema.

Este resumen aborda los conceptos clave de los datos, incluyendo las estructuras de datos, tipos de datos, formatos de almacenamiento, bases de datos y procesamiento de datos transaccionales.

## Tipos de Datos

### Datos Estructurados

Los **datos estructurados** son aquellos que se organizan en un formato bien definido, generalmente en tablas con filas y columnas que contienen información de un solo tipo. Estos datos son fáciles de almacenar y consultar, ya que tienen una estructura fija.

**Ejemplo**:

- Una base de datos relacional como MySQL, donde cada campo tiene un tipo específico (entero, cadena, fecha, etc.).

### Datos Semiestructurados

Los **datos semiestructurados** tienen una estructura flexible que permite variaciones entre diferentes instancias. A menudo se almacenan en formatos como JSON o XML, que utilizan etiquetas o jerarquías para organizar los datos, pero permiten variabilidad en la estructura de los registros.

**Ejemplo**:

{
  "customers": [
    {
      "firstName": "Joe",
      "lastName": "Jones",
      "contact": [
        {
          "type": "home",
          "number": "555 123-1234"
        },
        {
          "type": "email",
          "address": "joe@litware.com"
        }
      ]
    }
  ]
}

### Datos No Estructurados

Los **datos no estructurados** son aquellos que no tienen una organización predefinida y no pueden clasificarse fácilmente en tablas o estructuras de filas y columnas. Incluyen imágenes, audios, videos y documentos no formateados.

**Ejemplo**:

- Archivos de imágenes, grabaciones de audio y videos.

## Almacenamiento de Datos

El almacenamiento de datos depende del tipo de datos y de las necesidades del sistema. Existen varias opciones para almacenar datos de manera eficiente:

### Archivos de Texto Delimitados

Son archivos donde los datos están separados por delimitadores específicos, como comas o tabulaciones. El formato más común es CSV (Comma Separated Values), donde cada campo está separado por una coma y las filas por un salto de línea.

**Ejemplo**:

FirstName,LastName,Email  
Joe,Jones,joe@litware.com  
Samir,Nadoy,samir@northwind.com

### Formato JSON

El formato **JSON** (JavaScript Object Notation) es ampliamente utilizado por su simplicidad y capacidad para representar datos jerárquicos. Es legible tanto para máquinas como para humanos.

**Ejemplo**:

{
  "customers": [
    {
      "firstName": "Joe",
      "lastName": "Jones",
      "contact": [
        {
          "type": "home",
          "number": "555 123-1234"
        },
        {
          "type": "email",
          "address": "joe@litware.com"
        }
      ]
    }
  ]
}

### Formato XML

El formato **XML** (Extensible Markup Language) utiliza etiquetas para definir elementos y atributos, permitiendo representar datos jerárquicos. Aunque ha sido reemplazado en muchos casos por JSON, sigue siendo popular en ciertas aplicaciones.

**Ejemplo**:

<Customers>  
&nbsp;&nbsp;<Customer name="Joe" lastName="Jones">  
&nbsp;&nbsp;&nbsp;&nbsp;<ContactDetails>  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<Contact type="home" number="555 123-1234"/>  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<Contact type="email" address="joe@litware.com"/>  
&nbsp;&nbsp;&nbsp;&nbsp;</ContactDetails>  
&nbsp;&nbsp;</Customer>  
</Customers>

### Formato Avro

El formato **Avro** es un formato de datos basado en filas creado por Apache. Es eficiente en términos de almacenamiento y compresión, ideal para grandes volúmenes de datos.

**Ejemplo**:

- Un archivo Avro contiene el esquema de datos y los registros, permitiendo deserializar los datos con facilidad.

### Formato ORC

El formato **ORC** (Optimized Row Columnar) organiza los datos en columnas en lugar de filas. Mejora el rendimiento en bases de datos como Apache Hive para consultas analíticas de grandes volúmenes de datos.

### Formato Parquet

El formato **Parquet** es un formato de datos basado en columnas, altamente eficiente en compresión y codificación. Es ideal para consultas rápidas y análisis de grandes conjuntos de datos.

## Bases de Datos

### Bases de Datos Relacionales

Las bases de datos **relacionales** organizan los datos en tablas y utilizan **SQL** (Structured Query Language) para consultar y manipular los datos. Son adecuadas para datos estructurados.

**Ejemplo**:

- MySQL, PostgreSQL, Oracle.

### Bases de Datos No Relacionales (NoSQL)

Las bases de datos **NoSQL** no utilizan un esquema fijo, permitiendo almacenar datos más variados como documentos JSON, clave-valor o columnas. Son útiles para datos semiestructurados y no estructurados.

#### Tipos de Bases de Datos NoSQL:

1. **Clave-Valor**: Cada entrada es una clave única con un valor asociado.
2. **Documentos**: Almacenan datos en forma de documentos (generalmente JSON).
3. **Columnas**: Organizan datos en columnas, agrupadas en familias de columnas.
4. **Grafos**: Almacenan entidades como nodos con vínculos que representan relaciones.

**Ejemplo**:

- MongoDB (documentos), Redis (clave-valor), Cassandra (columnas).

## Procesamiento de Datos Transaccionales

El procesamiento de datos transaccionales, conocido como **OLTP** (Online Transaction Processing), se enfoca en operaciones de bases de datos que involucran grandes volúmenes de transacciones. Las transacciones deben seguir las propiedades **ACID**:

- **Atomicidad**: Cada transacción es una unidad indivisible.
- **Coherencia**: Los datos deben estar en un estado válido antes y después de la transacción.
- **Aislamiento**: Las transacciones simultáneas no interfieren entre sí.
- **Durabilidad**: Una vez confirmada, la transacción es permanente.

**Ejemplo**:

- Un sistema bancario que procesa transferencias de dinero entre cuentas.

## Conclusión

Comprender los tipos de datos, sus estructuras, formatos de almacenamiento y sistemas de bases de datos es esencial para diseñar e implementar soluciones tecnológicas eficientes. Cada tipo de dato y formato de almacenamiento tiene su propósito y aplicaciones, permitiendo optimizar el manejo y procesamiento de grandes volúmenes de datos en diversos contextos.
