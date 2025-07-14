

- Device Management
-  Authenticate 

Web Service Endpoint

# Authenticate

Authenticates a user during MDM payload installation.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/checkin#AuthenticateRequest
```

## HTTP Body

AuthenticateRequest

The request object for authentication.

Content-Type: application/x-apple-aspen-mdm-checkin

## Response Codes

` 200 ``OK`

`OK`

## Discussion

On success, the server must respond with a `200 OK` status. The server shouldn’t assume that the device has installed the MDM payload at this time, as other payloads in the profile may still fail to install. When the device has successfully installed the MDM payload, it sends a Token Update message.

## Topics

### Request

object AuthenticateRequest

The Authenticate Request details.

## See Also

### Commands

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

Set Bootstrap Token

Sets the bootstrap token.

