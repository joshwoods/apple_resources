

- Device Management
-  Assign Account-Driven Enrollment Service Discovery 

Web Service Endpoint

# Assign Account-Driven Enrollment Service Discovery

The Account-Driven Enrollment profile defines key attributes related to service discovery for account-driven enrollment, by MDM.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://mdmenrollment.apple.com/account-driven-enrollment/profile
```

## HTTP Body

AccountDrivenEnrollmentProfileRequest

The profile request for this account driven enrollment.

Content-Type: application/json

## Response Codes

` 200 ``OK`

`OK`

` 400 ``Bad Request`

`Bad Request`

- `MDM_SERVICE_DISCOVERY_URL_REQUIRED` - indicates that the MDM Service Discovery URL is missing in the request.

- `MDM_SERVICE_DISCOVERY_URL_NOT_VALID` - indicates that provided MDM Service Discovery URL may be incorrectly formatted or does not belong to the required HTTPS scheme.

- `ORG_NOT_SUPPORTED` - indicates that the associated org is not supported.

## Overview

This profile includes the MDM Service Discovery URL, which redirects users to the MDM to start the enrollment process during account-driven enrollment.

## Topics

### Supporting Request

object AccountDrivenEnrollmentProfileRequest

The details for an account driven enrollment profile.

## See Also

### Account-Driven Enrollment Service Discovery

Fetch Account-Driven Enrollment Service Discovery

Fetch the Account-Driven Enrollment profile set by MDM that includes information about service discovery for account-driven enrollment.

Remove Account-Driven Enrollment Profile

Remove the Account-Driven Enrollment profile set by MDM that includes information about service discovery for account-driven enrollment.

