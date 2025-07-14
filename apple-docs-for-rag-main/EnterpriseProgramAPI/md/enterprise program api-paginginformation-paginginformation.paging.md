

- Enterprise Program API
- PagingInformation
-  PagingInformation.Paging 

Object

# PagingInformation.Paging

Paging details such as the total number of resources and the per-page limit.

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

## Attributes 

Possible types:

## Discussion

Adjust the number of resources returned per page by using the `limit` query parameter in your request. For example, the following request returns the first 10 users:

```
GET /v1/users?limit=10
```

