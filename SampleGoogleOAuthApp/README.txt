It's not recommended to store secrets in config files, so I've saved them in the User Secret Storage.
Steps to set it up:
1. Run the following command in the project directory:
dotnet user-secrets init
2. Store client id and secret in the local secret store:
dotnet user-secrets set "Authentication:Google:ClientId" "<client-id>"
dotnet user-secrets set "Authentication:Google:ClientSecret" "<client-secret>"