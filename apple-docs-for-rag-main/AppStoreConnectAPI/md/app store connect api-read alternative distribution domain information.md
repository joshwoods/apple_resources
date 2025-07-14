

- App Store Connect API
-  Read alternative distribution domain information 

Web Service Endpoint

# Read alternative distribution domain information

Read information for a specific alternative distribution domain.

App Store Connect API 3.4.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/alternativeDistributionDomains/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `alternative distribution domain` resource ID from the List alternative distribution domains response.

## Query Parameters

`fields[alternativeDistributionDomains]`

`[string]`

Possible Values: `domain, referenceName, createdDate`

## Response Codes

` 200 ``OK`

AlternativeDistributionDomainResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
```

```
```

## See Also

### Managing domains

Add an alternative distribution domain

Add an alternative distribution domain to your account.

List alternative distribution domains

List all the alternative distribution domains for your account.

Delete an alternative distribution domain

Delete the alternative distribution search domain for an app.

Add a marketplace domain

Add an alternative marketplace domain to your account.

Deprecated

Read marketplace domain information

Read information for a specific alternative marketplace domain.

Deprecated

List marketplace domains

List all the alternative marketplace domains for your account.

Deprecated

Delete a marketplace domain

Delete the alternative marketplace search domain for an app.

Deprecated

