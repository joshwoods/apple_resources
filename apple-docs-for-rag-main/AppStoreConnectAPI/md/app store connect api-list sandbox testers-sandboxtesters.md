

- App Store Connect API
-  List Sandbox Testers 

Web Service Endpoint

# List Sandbox Testers

Get a list of Sandbox Testers for your team.

App Store Connect API 2.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v2/sandboxTesters
```

## Query Parameters

`fields[sandboxTesters]`

`[string]`

Possible Values: `firstName, lastName, acAccountName, territory, applePayCompatible, interruptPurchases, subscriptionRenewalRate`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

SandboxTestersV2Response

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
https://api.appstoreconnect.apple.com/v2/sandboxTesters
```

```
{
  "data" : [ {
    "type" : "sandboxTesters",
    "id" : "47be9e57-1a3f-49c2-8ce7-af27a977ebb0",
    "attributes" : {
      "firstName" : "Anne",
      "lastName" : "Johnson",
      "acAccountName" : "annejohnson1@icloud.com",
      "territory" : "USA",
      "applePayCompatible" : true,
      "interruptPurchases" : false,
      "subscriptionRenewalRate" : "MONTHLY_RENEWAL_EVERY_FIVE_MINUTES"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/sandboxTesters/47be9e57-1a3f-49c2-8ce7-af27a977ebb0"
    }
  } ],
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v2/sandboxTesters"
  },
  "meta" : {
    "paging" : {
      "total" : 1,
      "limit" : 50
    }
  }
}

```

## See Also

### Sandbox Tester Lookup and Modification

Modify a Sandbox Tester

Change the subscription renewal time rate, set interrupted purchases or change territory of Sandbox Apple Account.

Clear Purchase History for a Sandbox Tester

Remove purchase history from a Sandbox Apple Account.

