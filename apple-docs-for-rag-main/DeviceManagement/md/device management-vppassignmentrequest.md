

- Device Management
-  VppAssignmentRequest 

Object

# VppAssignmentRequest

The request for a list of assignments.

Device Assignment ServicesVPP License Management

``` source
object VppAssignmentRequest
```

## Properties

`adamIdStr`

`string`

The unique identifier for a product in the iTunes Store.

`clientUserIdStr`

`string`

If specified, returns only assignments assigned to the given client user ID.

`pageIndex`

`int32`

The index of the page to lookup. To page through the assignemnts, use the `nextPageIndex` value returned in the previous VppAssignmentsResponse.

This must be used in combination with a `requestID`, also from the previous response.

`requestId`

`string`

A unique ID that is used when making paginated requests.

`serialNumber`

`string`

If specified, returns only assignments assigned to the given serial number.

`sToken`

`string`

 (Required) 

The authentication token.

## See Also

### Request and Response

object VppAssignmentsResponse

The response that contains a list of assignments.

