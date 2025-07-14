

- Apple Search Ads
-  Get Me Details 

Web Service Endpoint

# Get Me Details

Fetches details of an API caller.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/me
```

## Response Codes

` 200 ``OK`

MeDetailResponse

`OK`

If the call succeeds, the API returns the MeDetail object in the response payload with an HTTP status code of 200 (OK). If unsuccessful, the HTTP status code indicates the error with details in the error message.

Content-Type: application/json

` 401 ``Unauthorized`

ApiErrorResponse

`Unauthorized`

An unauthenticated call fails to get the requested response.

Content-Type: application/json

` 403 ``Forbidden`

ApiErrorResponse

`Forbidden`

Insufficient rights to the resource.

Content-Type: application/json

` 429 `

ApiErrorResponse

The API calls exceed rate-limit thresholds. See the Rate Limits subsection of Calling the Apple Search Ads API.

Content-Type: application/json

` 500 ``Internal Server Error`

ApiErrorResponse

`Internal Server Error`

The Apple Search Ads server is temporarily down or unreachable. The request may be valid, but you need to retry it later.

Content-Type: application/json

## Mentioned in 

Apple Search Ads Campaign Management API 4

## Discussion

This endpoint returns the `userId` and `parentOrgId` of an API caller. See the MeDetail object.

### Get Me Details Example

- Request
- Response

```
curl "https://api.searchads.apple.com/api/v5/me"
-H "Authorization: Bearer {access_token}" \
-H "X-AP-Context: orgId={orgId}"
```

```
{
  "userId": 3962840,
  "parentOrgId": 27154130
}

```

## See Also

### Access Control List

Get User ACL

Fetches roles and organizations that the API has access to.

object UserAcl

The response to ACL requests.

object UserAclListResponse

A container for ACL call responses.

object MeDetail

The API caller identifiers.

object MeDetailResponse

The response from me detail calls.

