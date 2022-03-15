# ShoeStore

### Running the Sample
After cloning or downloading the project, you need to using database update commands (just below). Postgre SQL is used in the project.
```
* Update-Database -Context StoreContext
* Update-Database -Context AppIdentityDbContext
```
![image](https://raw.githubusercontent.com/burakyuz1/ShoeStore/main/usage.png?token=GHSAT0AAAAAABROC7M7YPGJREKLGVE3LERWYRQPESA)

### Project Structure
```
/src
* ApplicationCore
* Infrastructure
* Web

/tests
* UnitTests
```

### Migrations
```
/Infrastructure
Add-Migration InitialCreate -Context StoreContext -OutputDir "Data\Migrations"
Update-Database -Context StoreContext
Add-Migration InitialIdentity -Context AppIdentityDbContext -OutputDir "Identity\Migrations"
Update-Database -Context AppIdentityDbContext
```

### Packages
```
/ApplicationCore
Install-Package Ardalis.Specification -v 5.2.0

/Infrastructure
Install-Package Microsoft.EntityFrameworkCore -v 5.0.14
Install-Package Npgsql.EntityFrameworkCore.PostgreSQL -v 5.0.10
Install-Package Ardalis.Specification.EntityFrameworkCore -v 5.2.0
Install-Package Microsoft.AspNetCore.Identity.EntityFrameworkCore -v 5.0.14

/UnitTests
Install-Package Moq
```

### Resources
* https://github.com/yigith/TechMarket
* https://github.com/dotnet-architecture/eShopOnWeb
* https://www.connectionstrings.com/postgresql/
* https://docs.microsoft.com/en-us/aspnet/core/fundamentals/localization?view=aspnetcore-5.0#localization-middleware
* https://getbootstrap.com/docs/5.1/forms/layout/#inline-forms
* https://getbootstrap.com/docs/5.1/components/pagination/#alignment
* https://gist.github.com/yigith/c6f999788b833dc3d22ac6332a053dd1
* https://docs.microsoft.com/en-us/aspnet/core/fundamentals/http-context?view=aspnetcore-5.0
* https://docs.microsoft.com/en-us/ef/core/querying/related-data/eager
* https://docs.microsoft.com/en-us/aspnet/core/mvc/models/model-binding?view=aspnetcore-5.0#dictionaries-1
* https://github.com/dotnet/aspnetcore/issues/16663
* https://docs.microsoft.com/en-us/dotnet/api/microsoft.aspnetcore.mvc.modelbinderattribute.name?view=aspnetcore-5.0
* https://docs.microsoft.com/en-us/aspnet/core/fundamentals/middleware/write?view=aspnetcore-5.0
* https://getbootstrap.com/docs/5.1/examples/checkout/
* https://docs.microsoft.com/en-us/aspnet/core/mvc/views/view-components?view=aspnetcore-5.0
