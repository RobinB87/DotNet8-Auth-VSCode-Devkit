1) Create devcontainer
2) Ctrl + shift + p: .NET new project (ASP.NET Core Empty)

3) Add packages:
- cd src/Authentication
- dotnet add package Microsoft.AspNetCore.Identity.EntityFrameworkCore (version 8)
- dotnet add package Microsoft.EntityFrameworkCore.Sqlite --version (version 8)
- dotnet add package Microsoft.EntityFrameworkCore.Design --version (version 8)

4) Add migration:
- dotnet ef migrations add InitialCreate

5) dotnet ef database update