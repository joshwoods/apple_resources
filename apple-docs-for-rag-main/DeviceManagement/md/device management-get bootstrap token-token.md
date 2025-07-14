

- Device Management
-  Get Bootstrap Token 

Web Service Endpoint

# Get Bootstrap Token

Gets the bootstrap token.

macOS 10.15+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/checkin#GetBootstrapTokenRequest
```

## HTTP Body

GetBootstrapTokenRequest

The request object the app uses to get the bootstrap token.

Content-Type: application/x-apple-aspen-mdm-checkin

## Response Codes

` 200 ``OK`

GetBootstrapTokenResponse

`OK`

The response object that contains the bootstrap token.

Content-Type: application/xml

## Discussion

This command returns the bootstrap token data if it was previously set and the feature is enabled by the server.

If no bootstrap token is available, the server should return empty or no data and no error.

It requires a Device Enrollment Program enrolled client, or on macOS 11 and later, a supervised device.

## Topics

### Request and Response

object GetBootstrapTokenRequest

The request object used to get the bootstrap token.

object GetBootstrapTokenResponse

The response that contains the bootstrap token.

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

Set Bootstrap Token

Sets the bootstrap token.

