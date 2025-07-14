

- Device Management
-  Get All Storefronts 

Web Service Endpoint

# Get All Storefronts

Fetch all the storefronts in alphabetical order.

Device Assignment ServicesVPP License Management

## URL

``` source
GET https://api.ent.apple.com/v1/storefronts#all
```

## Query Parameters

`extend`

`[string]`

A list of attribute extensions to apply to resources in the response.

Classifier (optional): A resource type to apply the parameter to.

`include`

`[string]`

A list of relationship names to include for resources in the response.

Classifier (optional): A resource type to apply the parameter to.

`l`

`string`

The localization to use, which you specify with a language tag. The possible values are in the `supportedLanguageTags` array belonging to the `Storefront` object that `storefront` specifies. Otherwise, the default is `defaultLanguageTag` in `Storefront`.

`limit`

`integer`

A limit to apply to the results.

Classifier (optional): A relationship name to apply the limit to.

`offset`

`string`

The offset to use for a paginated request.

`relate`

`[string]`

A list of relationship names to relate for resources in the response.

Classifier (optional): A resource type to apply the parameter to.

`platform`

`string`

 (Required) 

The platform the user-facing app is running on. You use this to get metadata for the specified platform.

Possible Values: `appletv, ipad, iphone, mac, realityDevice, web`

## Response Codes

` 200 ``OK`

StorefrontsResponse

`OK`

The collection of storefronts for the request.

Content-Type: application/json

` 401 ``Unauthorized`

UnauthorizedResponse

`Unauthorized`

A response indicating an incorrect `Authorization` header.

Content-Type: application/json

` 500 ``Internal Server Error`

ErrorsResponse

`Internal Server Error`

A response indicating an error occurred on the server.

Content-Type: application/json

## See Also

### Requesting a catalog storefront

Get a Storefront

Fetch a single storefront by using its identifier.

Get Multiple Storefronts

Fetch one or more storefronts by using their identifiers.

