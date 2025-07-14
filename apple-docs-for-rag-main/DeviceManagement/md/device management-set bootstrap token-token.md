

- Device Management
-  Set Bootstrap Token 

Web Service Endpoint

# Set Bootstrap Token

Sets the bootstrap token.

macOS 10.15+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/checkin#SetBootstrapTokenRequest
```

## HTTP Body

SetBootstrapTokenRequest

The request object used to set the bootstrap token.

Content-Type: application/x-apple-aspen-mdm-checkin

## Response Codes

` 200 ``OK`

`OK`

## Discussion

This command changes or clears the bootstrap token data for the device.

It requires a Device Enrollment Program enrolled client, or on macOS 11 and later, a supervised device.

## Topics

### Request

object SetBootstrapTokenRequest

The request object used to set the bootstrap token.

## See Also

### Commands

Authenticate

Authenticates a user during MDM payload installation.

UserAuthenticate

Authenticates a user with a two-step authentication protocol.

Check Out

Responds to the removal of the MDM enrollment profile from a device.

Get Token

Check-in protocol get-token data.

Token Update

Updates the token for a device on the server.

Get Bootstrap Token

Gets the bootstrap token.

