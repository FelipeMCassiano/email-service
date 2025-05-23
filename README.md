# Email service

This project was built using C#, .NET Core and Amazon SES

![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=csharp&logoColor=white)
![.Net](https://img.shields.io/badge/.NET-5C2D91?style=for-the-badge&logo=.net&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)

## Instalation
1. Clone the repository
```bash
git clone https://github.com/FelipeMCassiano/desafio-backend-uber
```
2. Run ```dotnet restore```
3. Update `appsettings.Development.json` putting your AWS credentials
```json
{
  "Settings" : {
    "SES": {
      "AccessKey" : "**************",
      "SecretKey" : "**************************"
    }
  }
}
```
## Usage 
1. Start the app with ```bash dotnet run dotnet run --project /EmailService/src/Backend/EmailService.API
2. The api will be accessible at [http://localhost:5085/swagger/index.html](http://localhost:5085/swagger/index.html)

## API Endpoints
**SEND EMAIL**

```POST /emailservice/send ```

**BODY**
```json
{
  "to": "string",
  "subject": "string",
  "body": "string"
}
```
