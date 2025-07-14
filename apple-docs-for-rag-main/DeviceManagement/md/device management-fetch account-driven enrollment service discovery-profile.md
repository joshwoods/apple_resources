

- Device Management
-  Fetch Account-Driven Enrollment Service Discovery 

Web Service Endpoint

# Fetch Account-Driven Enrollment Service Discovery

Fetch the Account-Driven Enrollment profile set by MDM that includes information about service discovery for account-driven enrollment.

Device Assignment ServicesVPP License Management

## URL

``` source
GET https://mdmenrollment.apple.com/account-driven-enrollment/profile
```

## Response Codes

` 200 ``OK`

GetAccountDrivenEnrollmentProfileResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

- `ORG_NOT_SUPPORTED` - indicates that the associated org is not supported.

` 404 ``Not Found`

`Not Found`

- `NOT_FOUND` - indicates that MDM Service Discovery URL is not found.

## Topics

### Supporting Response

object GetAccountDrivenEnrollmentProfileResponse

The details for an account driven enrollment profile.

## See Also

### Account-Driven Enrollment Service Discovery

Assign Account-Driven Enrollment Service Discovery

The Account-Driven Enrollment profile defines key attributes related to service discovery for account-driven enrollment, by MDM.

Remove Account-Driven Enrollment Profile

Remove the Account-Driven Enrollment profile set by MDM that includes information about service discovery for account-driven enrollment.

