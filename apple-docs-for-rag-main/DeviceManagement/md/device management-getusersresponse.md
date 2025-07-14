

- Device Management
-  GetUsersResponse 

Object

# GetUsersResponse

The paginated response that contains the requested users.

Device Assignment ServicesVPP License Management

``` source
object GetUsersResponse
```

## Properties

`currentPageIndex`

`int32`

The current page index of the paginated response.

`nextPageIndex`

`int32`

The next page index in the paginated response.

The response only includes this field when there is a next page.

`size`

`int32`

The number of users on the current page.

`totalPages`

`int32`

The total number of pages in the paginated response.

`users`

`[`ResponseUser`]`

The set of requested users.

`versionId`

`string`

The current version identifier. When traversing the paginated response, use `versionId` to identify when changes occur to underlying data.

When any writes occur to the underlying data in a fetch, `versionId` updates.

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

Managing Apps and Books Through Web Services

## Topics

### Objects and Data Types

object ResponseUser

The user in the organization.

object MdmInfo

Information about the MDM client.

## See Also

### Response

object ErrorResponse

The response that contains the error that occurs.

