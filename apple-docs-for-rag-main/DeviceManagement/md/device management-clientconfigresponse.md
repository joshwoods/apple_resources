

- Device Management
-  ClientConfigResponse 

Object

# ClientConfigResponse

The response that contains the client configuration.

Device Assignment ServicesVPP License Management

``` source
object ClientConfigResponse
```

## Properties

`countryISO2ACode`

`string`

The ISO alpha-2 country code that designates the organization’s location.

`defaultPlatform`

`string`

The value that the MDM client passes for the platform parameter in the `contentMetadataLookup` request. For more information about how the MDM client queries metadata by using `contentMetadataLookup`, see Getting App and Book Information (Legacy).

Possible Values: `volumestore, enterprisestore`

`notificationUrl`

`string`

The current URL to post notifications to.

`subscribedNotificationTypes`

`[string]`

The set of currently subscribed notification types.

Possible Values: `ASSET_MANAGEMENT, USER_MANAGEMENT, USER_ASSOCIATED, ASSET_COUNT`

`websiteURL`

`string`

The current website URL for the specified platform.

Possible Values: `https://school.apple.com, https://business.apple.com`

`mdmInfo`

MdmInfo

The current information for the provided token.

The response only includes this field when the MDM client sets a value using the Client Config endpoint.

`notificationAuthToken`

`string`

The current shared secret that the server returns in the Authorization header of notifications.

`tokenExpirationDate`

`string`

The token’s expiration date in an ISO-8601 format.

Note: The server shows all dates and times in UTC.

`uId`

`string`

The unique library identifier. When querying records using multiple tokens that may share libraries, use the `uId` field to filter duplicates and avoid double-counting records when different content managers upload duplicate tokens.

`locationName`

`string`

The current name of the library.

## Discussion

Client config should be checked regularly in order to verify expected values for the various fields.

## Topics

### Content Metadata

Apps and Books for Organizations

Get details about apps and books to show to your users.

## See Also

### Request and Response

object ClientConfigRequest

The request for the client configuration.

object ErrorResponse

The response that contains the error that occurs.

