

- Device Management
-  StatusResponse 

Object

# StatusResponse

The response that contains the event status.

Device Assignment ServicesVPP License Management

``` source
object StatusResponse
```

## Properties

`eventStatus`

`string`

The current status of the asynchronous event.

Possible Values: `PENDING, COMPLETE, FAILED`

`eventType`

`string`

The type of asynchronous event.

Possible Values: `ASSOCIATE, DISASSOCIATE, REVOKE, CREATE, UPDATE, RETIRE`

`failures`

`[`ErrorResponse`]`

Information regarding asynchronous failures.

`numCompleted`

`int32`

The number of completed tasks from the request.

`numRequested`

`int32`

The total number of tasks from the request.

`mdmInfo`

MdmInfo

The current information for the provided token.

The response only includes this field when MDM sets a value using the Client Config endpoint.

`tokenExpirationDate`

`string`

The token expiration date in an ISO-8601 format.

Note: The server shows all dates and times in UTC.

`uId`

`string`

The unique library identifier. When querying records using multiple tokens that may share libraries, use the `uId` field to filter duplicates and avoid double-counting records when different content managers upload duplicate tokens.

## Mentioned in 

Managing Assets

Managing Users

Handling Error Responses

## Topics

### Objects and Data Types

object ErrorResponse

The response that contains the error that occurs.

object MdmInfo

Information about the MDM client.

## See Also

### Response

object ErrorResponse

The response that contains the error that occurs.

