

- Device Management
-  Discover Authentication Servers 

Web Service Endpoint

# Discover Authentication Servers

Get a list of available authentication servers.

Device Assignment ServicesVPP License Management

## URL

``` source
GET https://yourmdmhost.example.com/.well-known/com.apple.remotemanagement
```

## Query Parameters

`model-family`

`string`

Possible Values: `Mac, iPhone, iPad, AppleTV, Watch, RealityDevice`

`user-identifier`

`string`

## Response Codes

` 200 ``OK`

WellKnown

`OK`

A list of servers the client device can use for authentication.

Content-Type: application/json

## Discussion

Each server entry corresponds to a server that supports a different version of the protocol. The client selects the server with the most recent version that matches its own most recent supported version.

## Topics

### Supporting Objects

object WellKnown

A list of available servers used for authentication.

## See Also

### Essentials

Onboarding users with account sign-in

Examine new, user-initiated, identity-focused flows.

object EnrollmentSSODocument

Enrollment SSO streamlines the MDM enrollment process, reduces sign-ins, and improves security.

