# SampleGoogleOAuthApp

This is a sample ASP.NET Core 6.0 MVC application with Google authentication.

To run it you must have Google ClienId and Client Secret. Please see instructions on how to get them: https://learn.microsoft.com/en-us/aspnet/core/security/authentication/social/google-logins?view=aspnetcore-8.0#create-the-google-oauth-20-client-id-and-secret

Then they must be added to the app configuration in appsettings.Development.json (not recommended), or in environment variables, or in User Secret Storage.

These are steps on how to add them to User Secrets:
1. Run the following command in the project directory:
```
dotnet user-secrets init
```
2. Store client id and secret in the local secret store:
```
dotnet user-secrets set "Authentication:Google:ClientId" "<client-id>"
dotnet user-secrets set "Authentication:Google:ClientSecret" "<client-secret>"
```
