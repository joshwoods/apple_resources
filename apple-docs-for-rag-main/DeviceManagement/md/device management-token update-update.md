

- Device Management
-  Token Update 

Web Service Endpoint

# Token Update

Updates the token for a device on the server.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/checkin#TokenUpdateRequest
```

## HTTP Body

TokenUpdateRequest

The request object for sending the new token.

Content-Type: application/x-apple-aspen-mdm-checkin

## Response Codes

` 200 ``OK`

`OK`

## Topics

### Request

object TokenUpdateRequest

The request object for sending the new token details.

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

Get Bootstrap Token

Gets the bootstrap token.

Set Bootstrap Token

Sets the bootstrap token.

