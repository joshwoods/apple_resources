

- Device Management
-  Get Account Detail 

Web Service Endpoint

# Get Account Detail

Obtain the details for your account.

Device Assignment ServicesVPP License Management

## URL

``` source
GET https://mdmenrollment.apple.com/account
```

## Response Codes

` 200 ``OK`

AccountDetail

`OK`

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

## Discussion

Each Mobile Device Management server must be registered with Apple. This endpoint provides details about the server entity to identify it uniquely throughout your organization. Each server is identifiable by either its system-generated unique identifier or by a user-provided name assigned by one of the organization’s users. Both the identifier and server name must be unique within your organization.

## Topics

### Response

object AccountDetail

The response that contains the details for an account.

