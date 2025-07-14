

- App Store Connect API
-  List alternative distribution domains 

Web Service Endpoint

# List alternative distribution domains

List all the alternative distribution domains for your account.

App Store Connect API 3.4.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/alternativeDistributionDomains
```

## Query Parameters

`fields[alternativeDistributionDomains]`

`[string]`

Possible Values: `domain, referenceName, createdDate`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

AlternativeDistributionDomainsResponse

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

Read alternative distribution domain information

Read information for a specific alternative distribution domain.

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

