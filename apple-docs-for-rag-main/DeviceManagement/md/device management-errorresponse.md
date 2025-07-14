

- Device Management
-  ErrorResponse 

Object

# ErrorResponse

The response that contains the error that occurs.

Device Assignment ServicesVPP License Management

``` source
object ErrorResponse
```

## Properties

`errorInfo`

ResponseErrorInfo

The request-specific information regarding the failure.

`errorMessage`

`string`

The human-readable error message that describes the failure.

`errorNumber`

`int32`

The error number that represents the failure.

## Mentioned in 

Handling Error Responses

## Topics

### Objects and Data Types

object ResponseErrorInfo

Information about the error.

## See Also

### Request and Response

object ManageAssetsRequest

The request for asset management.

object EventResponse

The response that contains the event identifier.

