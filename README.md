# 📚 Sistema de Biblioteca - Java Swing MVC

Este repositorio contiene un conjunto de proyectos Java organizados como multi-proyecto, desarrollados en NetBeans y usando una base de datos MySQL para la persistencia de datos. Anteriormente utilizaba archivos JSON, pero se ha migrado a una solución basada en base de datos relacional.

---

## 📦 Estructura del Proyecto
```
bibliotecaumg/
├── bibliotecaumg-app
├── bibliotecaumg-controladores
├── bibliotecaumg-datasources
├── bibliotecaumg-dto
├── bibliotecaumg-modelo
├── bibliotecaumg-utils
├── bibliotecaumg-vista
├── pom.xml
└── README.md
```
    
## 🚀 Instrucciones para Clonar e Instalar

1. **Clonar el repositorio:**

```bash
git clone https://github.com/tu-usuario/BibliotecaUMG.git
```

2. **Abrir en NetBeans:**

- Abre NetBeans.
- Ve a Archivo > Abrir Proyecto.
- Navega a la carpeta donde clonaste el repo.
- Selecciona los proyectos `biblioteca-model`, `biblioteca-database` y `biblioteca-vista`.

3. **Configurar Base de Datos MySQL:**

- Crea una base de datos llamada `biblioteca_umg`.
- Ejecuta el script `schema.sql` si está disponible.
- Asegúrate de que las credenciales en la clase `Conexion.java` coincidan:

```java
private static final String URL = "jdbc:mysql://localhost:3306/biblioteca_umg";
private static final String USER = "tu_usuario";
private static final String PASSWORD = "tu_contraseña";
```

## 🗂️ Requisitos

- JDK 17+
- NetBeans 15+
- MySQL 8.x
- Driver JDBC para MySQL (generalmente incluido en NetBeans o gestionado por Maven)

## ✅ Estado Actual

- ✅ Migrado a estructura multi-proyecto
- ✅ Persistencia migrada de JSON a MySQL
- ✅ Interfaz gráfica funcional
- ⚙️ Funcionalidad de préstamos y devoluciones (en desarrollo)

## 🧩 Notas Adicionales

- Puedes crear usuarios y libros directamente desde la interfaz.
- La base de datos debe estar activa antes de ejecutar la aplicación.
- Usa `.gitignore` para evitar subir configuraciones locales o credenciales.

## 🧑‍💻 Autores

- William Garcia
- Julio Lemus
- Oscar Gonzalez
- Bryan Mundo

## 📄 Licencia

Este proyecto es de uso académico y puede ser modificado con fines educativos. No se permite su redistribución comercial sin autorización previa.
