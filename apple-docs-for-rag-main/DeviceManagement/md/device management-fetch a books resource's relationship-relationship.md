

- Device Management
-  Fetch a books resource's relationship 

Web Service Endpoint

# Fetch a books resource's relationship

Device Assignment ServicesVPP License Management

## URL

``` source
GET https://api.ent.apple.com/v1/catalog/{storefront}/books/{id}/{relationship}
```

## Path Parameters

`id`

`string`

 (Required) 

`relationship`

`string`

 (Required) 

Value: `genres`

`storefront`

`string`

 (Required) 

## Query Parameters

`additionalPlatforms`

`[string]`

Possible Values: `appletv, ipad, iphone, mac, realityDevice, web`

`extend`

`[string]`

`include`

`[string]`

`l`

`string`

`limit`

`integer`

`platform`

`string`

 (Required) 

Possible Values: `appletv, ipad, iphone, mac, realityDevice, web`

`relate`

`[string]`

## Response Codes

` 200 ``OK`

RelationshipResponse

`OK`

Content-Type: application/json

` 401 ``Unauthorized`

UnauthorizedResponse

`Unauthorized`

Content-Type: application/json

` 500 ``Internal Server Error`

ErrorsResponse

`Internal Server Error`

Content-Type: application/json

## See Also

### Endpoints

Fetch a apps resource's relationship

Get Multiple Genres

Fetch metadata for genres from the catalog by using their identifiers.

Get a Genre

Fetch metadata for a genre from the catalog by using its identifier.

