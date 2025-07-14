

- Device Management
-  ErrorCodePairingTokenMissing 

Object

# ErrorCodePairingTokenMissing

An error response that indicates a missing pairing token.

watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ErrorCodePairingTokenMissing
```

## Properties

`code`

`string`

 (Required) 

Indicates that the pairing token, which the system requires to enroll the watch, is missing.

Value: `com.apple.watch.pairing.token.missing`

`description`

`string`

A description of the error. Only use this for logging purposes and don’t display it to the user.

`details`

ErrorCodePairingTokenMissing.Details

 (Required) 

A description of the error to display to the user.

`message`

`string`

A dictionary that contains additional data about the error code.

## Discussion

The schema for a JSON or property list XML document that an MDM server’s 403 response body contains. The response headers need to include a “Content-Type” header that indicates whether the response returns JSON or XML.

The system returns this response when an Apple Watch attempts to enroll in MDM, but the watch doesn’t include a `PAIRING_TOKEN` in the MachineInfo request. After the watch receives this response, it fetches a pairing token from the phone’s MDM server through a request to the phone. Then, the watch repeats the enrollment request and includes the pairing token.

## Topics

### Details

object ErrorCodePairingTokenMissing.Details

A dictionary that contains additional data about the token-missing error code.

