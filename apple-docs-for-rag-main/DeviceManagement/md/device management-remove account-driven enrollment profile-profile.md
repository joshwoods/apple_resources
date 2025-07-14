

- Device Management
-  Remove Account-Driven Enrollment Profile 

Web Service Endpoint

# Remove Account-Driven Enrollment Profile

Remove the Account-Driven Enrollment profile set by MDM that includes information about service discovery for account-driven enrollment.

Device Assignment ServicesVPP License Management

## URL

``` source
DELETE https://mdmenrollment.apple.com/account-driven-enrollment/profile
```

## Response Codes

` 200 ``OK`

`OK`

` 400 ``Bad Request`

`Bad Request`

- `ORG_NOT_SUPPORTED` - indicates that the associated org is not supported.

## See Also

### Account-Driven Enrollment Service Discovery

Assign Account-Driven Enrollment Service Discovery

The Account-Driven Enrollment profile defines key attributes related to service discovery for account-driven enrollment, by MDM.

Fetch Account-Driven Enrollment Service Discovery

Fetch the Account-Driven Enrollment profile set by MDM that includes information about service discovery for account-driven enrollment.

