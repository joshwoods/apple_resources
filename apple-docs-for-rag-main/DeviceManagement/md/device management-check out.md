

- Device Management
-  Check Out 

Web Service Endpoint

# Check Out

Responds to the removal of the MDM enrollment profile from a device.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/checkin#CheckOutRequest
```

## HTTP Body

CheckOutRequest

The request object for check out.

Content-Type: application/x-apple-aspen-mdm-checkin

## Response Codes

` 200 ``OK`

`OK`

## Discussion

This message is sent on a best-effort basis. If the message cannot be sent while the profile is being removed, the MDM profile will be removed, and the message will not be resent.

On success, the server must respond with a `200 OK` status.

## Topics

### Request

object CheckOutRequest

The Check Out Request details.

## See Also

### Commands

Authenticate

Authenticates a user during MDM payload installation.

UserAuthenticate

Authenticates a user with a two-step authentication protocol.

Get Token

Check-in protocol get-token data.

Token Update

Updates the token for a device on the server.

Get Bootstrap Token

Gets the bootstrap token.

Set Bootstrap Token

Sets the bootstrap token.

