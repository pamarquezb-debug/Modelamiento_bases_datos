# Modelamiento de Bases de Datos - Semana 7

## DUOC UC

**Asignatura:** Modelamiento de Bases de Datos  
**Semana:** 7  
**Actividad:** Realizando el poblamiento y consultas en la base de datos con sentencias SQL  
**Caso:** Holding Carpenter SPA  
**Base de datos:** Oracle Database  
**Herramienta:** Oracle SQL Developer / Oracle Cloud  

---

## Descripción

Este repositorio contiene el desarrollo de la actividad correspondiente a la Semana 7 de la asignatura Modelamiento de Bases de Datos.

El caso plantea la implementación de una base de datos para el Holding Carpenter SPA, destinada a administrar información relacionada con las compañías y su personal.

La solución fue desarrollada mediante sentencias SQL y probada utilizando Oracle Cloud.

---

## Contenido de la actividad

El script SQL contempla los siguientes casos:

### Caso 1 - Implementación del modelo

Creación de las tablas del modelo relacional y definición de:

- Claves primarias (PK)
- Claves foráneas (FK)
- Claves únicas (UN)
- Restricciones CHECK (CK)
- Relaciones entre las tablas

También se utilizan columnas `IDENTITY` para la generación automática de identificadores en las tablas correspondientes.

### Caso 2 - Modificación del modelo

Mediante sentencias `ALTER TABLE` se incorporan las siguientes reglas de negocio:

- El correo electrónico del personal es opcional, pero no puede repetirse.
- El dígito verificador del RUN solo puede contener valores entre 0 y 9 o la letra K.
- El sueldo mínimo permitido para el personal es de $450.000.

### Caso 3 - Poblamiento del modelo

Se realiza el poblamiento de las tablas solicitadas:

- REGION
- COMUNA
- IDIOMA
- COMPANIA

Para la generación de identificadores se utilizan:

- `IDENTITY` para REGION e IDIOMA.
- `SEQUENCE` para COMUNA y COMPANIA.

### Caso 4 - Recuperación de datos

Se desarrollan dos consultas SQL:

**Informe 1:** Simulación de la renta promedio de las empresas aplicando el porcentaje de aumento correspondiente.

**Informe 2:** Nueva simulación salarial agregando un 15% adicional al porcentaje de aumento registrado para cada empresa.

Las consultas utilizan alias, cálculos y ordenamiento de datos según los requerimientos planteados.

---

## Archivo principal

```text
PRY2204_S7_Holding_Carpenter.sql
```

El archivo contiene:

```text
DDL
├── CREATE TABLE
├── PRIMARY KEY
├── FOREIGN KEY
├── UNIQUE
└── CHECK

DML
└── INSERT INTO

Objetos Oracle
├── IDENTITY
└── SEQUENCE

Consultas
└── SELECT
```

---

## Ejecución

1. Ingresar a Oracle SQL Developer u Oracle Cloud.
2. Conectarse utilizando el usuario correspondiente a la Semana 7.
3. Abrir el archivo:

```text
PRY2204_S7_Holding_Carpenter.sql
```

4. Ejecutar el script completo.
5. Verificar la creación y poblamiento de las tablas.
6. Ejecutar los informes incluidos al final del script.

---

## Validación

El script fue ejecutado y probado en Oracle Cloud sin presentar errores.

---

## Autor

**Pablo Márquez**  
Duoc UC  
2026
