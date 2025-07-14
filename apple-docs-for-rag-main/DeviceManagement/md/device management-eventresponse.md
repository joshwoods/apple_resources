

- Device Management
-  EventResponse 

Object

# EventResponse

The response that contains the event identifier.

Device Assignment ServicesVPP License Management

``` source
object EventResponse
```

## Properties

`eventId`

`string`

The unique identifier for the asynchronous event.

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

## Topics

### Objects and Data Types

object MdmInfo

Information about the MDM client.

## See Also

### Request and Response

object ManageAssetsRequest

The request for asset management.

object ErrorResponse

The response that contains the error that occurs.

