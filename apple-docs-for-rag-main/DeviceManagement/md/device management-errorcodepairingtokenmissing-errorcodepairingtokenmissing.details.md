

- Device Management
- ErrorCodePairingTokenMissing
-  ErrorCodePairingTokenMissing.Details 

Object

# ErrorCodePairingTokenMissing.Details

A dictionary that contains additional data about the token-missing error code.

watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ErrorCodePairingTokenMissing.Details
```

## Properties

`security-token`

`string`

 (Required) 

The security token to pass to the phone’s MDM server to create the pairing token. This token needs to be a random UUID string.

