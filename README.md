# Customize ASP.NET Core Identity and Change ID from String to GUID

This is a sample ASP.NET Core web application that demonstrates how to customize ASP.NET Core Identity by changing the ID field from string to GUID. By default, ASP.NET Core Identity uses a string for the ID field in its user and role models. However, in some cases, it may be necessary to use a GUID instead of a string for the ID field.

In this project, we create a custom `ApplicationUser` class that inherits from `IdentityUser<Guid>`, which allows us to use GUIDs for user IDs. We also create a custom `ApplicationDbContext` class that inherits from `IdentityDbContext<ApplicationUser>` and configures ASP.NET Core Identity to use our custom `ApplicationUser` class.

This project provides an example of how to customize ASP.NET Core Identity to use GUIDs for IDs. Feel free to use this code as a starting point for your own projects that require GUIDs for user IDs.

## Getting Started

To run this project, you will need Visual Studio 2019 and .NET Core 3.1 or later installed on your machine. You can clone this repository or download the ZIP file to your local machine.

Once you have the project on your machine, open the `IdentityTest.sln` solution file in Visual Studio and run the project. You can then navigate to `https://localhost:5001` in your web browser to see the application in action.

## References

- [ASP.NET Core Identity documentation](https://docs.microsoft.com/en-us/aspnet/core/security/authentication/identity)
- [Microsoft.AspNetCore.Identity.EntityFrameworkCore namespace](https://docs.microsoft.com/en-us/dotnet/api/microsoft.aspnetcore.identity.entityframeworkcore?view=aspnetcore-5.0)

