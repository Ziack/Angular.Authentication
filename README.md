# Angular.Authentication

##Register API##
http://ngauthenticationapi.azurewebsites.net/api/account/register | POST
###Headers###
| Name         | Value |
|--------------|------------------|
| Accept       | application/json |
| Content-Type | application/json |

###Payload###

```json
{
  "userName": "jdoe",
  "password": "SuperPass",
  "confirmPassword": "SuperPass"
}
```

##Register API##
http://ngauthenticationapi.azurewebsites.net/token| POST
###Headers###
| Name         | Value |
|--------------|------------------|
| Accept       | application/json |
| Content-Type | x-www-form-urlencoded |

###Payload###

| Name         | Value |
|--------------|------------------|
| grant_type   | password         |
| username     | {username}       |
| password     | {password}       |

##Orders API##
http://ngauthenticationapi.azurewebsites.net/api/orders| GET
###Headers###
| Name         | Value |
|--------------|------------------|
| Accept       | application/json |
| Content-Type | application/json |
| Authorization | Bearer {token} |
