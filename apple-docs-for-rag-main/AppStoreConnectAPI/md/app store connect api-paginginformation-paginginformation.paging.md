

- App Store Connect API
- PagingInformation
-  PagingInformation.Paging 

Object

# PagingInformation.Paging

Paging details such as the total number of resources and the per-page limit.

App Store Connect API 1.0+

``` source
object PagingInformation.Paging
```

## Properties

`total`

`integer`

The total number of resources matching your request.

`limit`

`integer`

 (Required) 

The maximum number of resources to return per page, from 0 to 200.

## Discussion

Adjust the number of resources returned per page by using the `limit` query parameter in your request. For example, the following request returns the first 10 testers:

```
GET /v1/betaTesters?limit=10
```

