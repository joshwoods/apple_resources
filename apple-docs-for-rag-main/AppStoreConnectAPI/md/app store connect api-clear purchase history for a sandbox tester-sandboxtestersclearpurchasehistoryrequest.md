

- App Store Connect API
-  Clear Purchase History for a Sandbox Tester 

Web Service Endpoint

# Clear Purchase History for a Sandbox Tester

Remove purchase history from a Sandbox Apple Account.

App Store Connect API 2.2+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v2/sandboxTestersClearPurchaseHistoryRequest
```

## HTTP Body

SandboxTestersClearPurchaseHistoryRequestV2CreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

SandboxTestersClearPurchaseHistoryRequestV2Response

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v2/sandboxTestersClearPurchaseHistoryRequest 
-d
{
  "data": {
    "type": "sandboxTestersClearPurchaseHistoryRequest",
    "relationships": {
      "sandboxTesters": {
        "data": [
          {
            "id": "47be9e57-1a3f-49c2-8ce7-af27a977ebb0",
            "type": "sandboxTesters"
          }
        ]
      }
    }
  }
}

```

```
{
  "data" : {
    "type" : "sandboxTestersClearPurchaseHistoryRequest",
    "id" : "c47f2eda-042e-4f4b-9bb9-ded24c507e41",
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/sandboxTestersClearPurchaseHistoryRequest/c47f2eda-042e-4f4b-9bb9-ded24c507e41"
    }
  },
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v2/sandboxTestersClearPurchaseHistoryRequest"
  }
}
```

## See Also

### Sandbox Tester Lookup and Modification

List Sandbox Testers

Get a list of Sandbox Testers for your team.

Modify a Sandbox Tester

Change the subscription renewal time rate, set interrupted purchases or change territory of Sandbox Apple Account.

