

- Apple Search Ads
-  Get User ACL 

Web Service Endpoint

# Get User ACL

Fetches roles and organizations that the API has access to.

Search Ads 5.0+

## URL

``` source
GET https://api.searchads.apple.com/api/v5/acls
```

## Response Codes

` 200 ``OK`

UserAclListResponse

`OK`

If successful, the API returns a list of ACL objects in the response payload with an HTTP status code of `200 (OK)`. If unsuccessful, the HTTP status code indicates the error with details in the error message.

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

## Discussion

The API uses a user access control list (ACL) for policy-based authorization to determine access to resources. The Get User ACL call fetches roles in all organizations. Each role has access to all organizations or a subset of them.

### Get user ACL example

- Request
- Response

```
GET https://api.searchads.apple.com/api/v5/acls
```

```
{
  "orgName": "Trip Trek",
  "orgId": 40669820,
  "currency": "USD",
  "timeZone": “America/Los_Angeles”,
  "paymentModel": "PAYG",
  "roleNames": [
    "Admin"
  ],
  "parentOrgId": “27154130”,
  "displayName": "Trip Trek"
}
```

### Campaign Groups

The API treats your `orgId` like a campaign group. If you need to manage Search Ads for multiple clients, or if you need to restrict user access to a subset of your campaigns, you can create additional campaign groups within your account. Otherwise, you can create and manage all your campaigns under your default `orgId` and campaign group.

## See Also

### Access Control List

object UserAcl

The response to ACL requests.

object UserAclListResponse

A container for ACL call responses.

Get Me Details

Fetches details of an API caller.

object MeDetail

The API caller identifiers.

object MeDetailResponse

The response from me detail calls.

