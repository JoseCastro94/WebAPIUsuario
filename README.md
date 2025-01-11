Paso 1: Instalar los Paquetes Necesarios

☑️ Microsoft.EntityFrameworkCore
☑️ Microsoft.EntityFrameworkCore.Sql
☑️ Microsoft.EntityFrameworkCore.Tools

☑️ Swashbuckle.AspNetCore
☑️ Swashbuckle.AspNetCore.Swagger

PASO 2. Ejecutar en la consola del Administrador de Paquetes

Scaffold-DbContext "Data Source=(local);Database=db_usuario;Trusted_Connection=True;TrustServerCertificate=True;" Microsoft.EntityFrameworkCore.SqlServer -OutputDir Models -Force


