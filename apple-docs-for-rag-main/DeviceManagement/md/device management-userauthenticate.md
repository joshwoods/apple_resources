

- Device Management
-  UserAuthenticate 

Web Service Endpoint

# UserAuthenticate

Authenticates a user with a two-step authentication protocol.

macOS 10.7+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/checkin#UserAuthenticateRequest
```

## HTTP Body

UserAuthenticateRequest

The request object for two-step user authentication.

Content-Type: application/x-apple-aspen-mdm-checkin

## Response Codes

` 200 ``OK`

`OK`

## Discussion

A UserAuthenticate handshake usually consists of two transactions between client and server. Upon receiving the first request from the client, the server should respond with a 200 status code and a dictionary containing a `DigestChallenge` key (string).

A zero-length `DigestChallenge` provided by the server indicates that the server does not require any `AuthToken` to be generated for this user. Otherwise, the client generates a digest from the user’s short name, the user’s clear-text password and the `DigestChallenge` value provided by the server. The resulting digest is sent in a second UserAuthenticate request to the server, which validates the response and returns a dictionary that contains an `AuthToken` value that is sent subsequent commands on the user channel (to both the `ServerURL` and `CheckInURL`).

If the server rejects the `DigestResponse` value because of an invalid password, it must return a `200` response and an empty `AuthToken` value. If the server does not want to mange this user, it returns a `410` status code to the initial `UserAuthenticate` request. The client will not make any additional requests to the server on behalf of this user for the duration of this login session.

The next time the user logs in, the client sends a new request and the server can optionally return `410` again. The `AuthToken` remains valid until the next time the client sends a UserAuthenticate request. The client initiates a handshake each time a mobile or network user logs in.

## Topics

### Request

object UserAuthenticateRequest

The User Authenticate Request details.

## See Also

### Commands

Authenticate

Authenticates a user during MDM payload installation.

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

