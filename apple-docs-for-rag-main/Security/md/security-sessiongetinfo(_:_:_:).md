

- Security
-  SessionGetInfo(\_:\_:\_:) 

Function

# SessionGetInfo(\_:\_:\_:)

Obtains information about a security session.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SessionGetInfo(
    _ session: SecuritySessionId,
    _ sessionId: UnsafeMutablePointer?,
    _ attributes: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`session`  

The session you are asking about. You can use one of the special sessions given in Session ID Values, for example to ask about your own session.

`sessionId`  

A pointer to a SecuritySessionId value that the function populates with the actual session ID for the session you asked about. This value will not be one of the special values from Session ID Values, but will instead be an actual session ID.

`attributes`  

A pointer to a SessionAttributeBits structure that the function fills with the attribute bits for the session.

## Return Value

A result code. See Sessions API Result Codes.

## Discussion

You can ask about any session whose identifier you know. Use the callerSecuritySession constant to ask about your own session (the one your process is in).

