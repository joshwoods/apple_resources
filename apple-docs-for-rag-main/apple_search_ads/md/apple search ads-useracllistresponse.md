

- Apple Search Ads
-  UserAclListResponse 

Object

# UserAclListResponse

A container for ACL call responses.

Search Ads 2.0+

``` source
object UserAclListResponse
```

## Properties

`data`

`[`UserAcl`]`

Response data that the API provides.

`error`

ErrorResponseBody

Error response data that the API provides.

`pagination`

PageDetail

Page detail information that the API provides.

## See Also

### Access Control List

Get User ACL

Fetches roles and organizations that the API has access to.

object UserAcl

The response to ACL requests.

Get Me Details

Fetches details of an API caller.

object MeDetail

The API caller identifiers.

object MeDetailResponse

The response from me detail calls.

