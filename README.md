Paso 1: Instalar los Paquetes Necesarios

☑️ Microsoft.EntityFrameworkCore
☑️ Microsoft.EntityFrameworkCore.Sql
☑️ Microsoft.EntityFrameworkCore.Tools

☑️ Swashbuckle.AspNetCore
☑️ Swashbuckle.AspNetCore.Swagger

PASO 2. Ejecutar en la consola del Administrador de Paquetes

Scaffold-DbContext "Data Source=(local);Database=db_usuario;Trusted_Connection=True;TrustServerCertificate=True;" Microsoft.EntityFrameworkCore.SqlServer -OutputDir Models -Force

◥◣◥◣◥◣ BASE DE DATOS - SQL SERVER ◥◣◥◣◥◣

CREATE DATABASE db_usuario
GO

USE db_usuario
GO

CREATE TABLE Usuario(
 id INT PRIMARY KEY IDENTITY,
 nombres VARCHAR(50) NOT NULL,
 apellidos VARCHAR(50) NOT NULL,
 correo VARCHAR(100) NOT NULL,
 username VARCHAR(100),
 fecha_creacion DATETIME
)
GO 

INSERT INTO Usuario VALUES('Juan Carlos','Sanchez Calderon', 'juan.sanchez@gmail.com','juan12',GETDATE())

SELECT * FROM usuario
GO
