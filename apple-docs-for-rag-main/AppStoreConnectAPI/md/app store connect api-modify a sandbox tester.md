

- App Store Connect API
-  Modify a Sandbox Tester 

Web Service Endpoint

# Modify a Sandbox Tester

Change the subscription renewal time rate, set interrupted purchases or change territory of Sandbox Apple Account.

App Store Connect API 2.2+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v2/sandboxTesters/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the Sandbox Tester resource ID from the List Sandbox Testers response

## HTTP Body

SandboxTesterV2UpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

SandboxTesterV2Response

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Discussion

Note

Changes that you make to product metadata with the App Store Connect API can take up to 1 hour to appear in the sandbox environment.

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v2/sandboxTesters/47be9e57-1a3f-49c2-8ce7-af27a977ebb0
```

```
{
  "data" : {
    "type" : "sandboxTesters",
    "id" : "47be9e57-1a3f-49c2-8ce7-af27a977ebb0",
    "attributes" : {
      "firstName" : "Anne",
      "lastName" : "Johnson",
      "acAccountName" : "annejohnson1@icloud.com",
      "territory" : "CAN",
      "applePayCompatible" : true,
      "interruptPurchases" : false,
      "subscriptionRenewalRate" : "MONTHLY_RENEWAL_EVERY_THIRTY_MINUTES"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v2/sandboxTesters/47be9e57-1a3f-49c2-8ce7-af27a977ebb0"
    }
  },
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v2/sandboxTesters/47be9e57-1a3f-49c2-8ce7-af27a977ebb0"
  }
}

```

## See Also

### Sandbox Tester Lookup and Modification

List Sandbox Testers

Get a list of Sandbox Testers for your team.

Clear Purchase History for a Sandbox Tester

Remove purchase history from a Sandbox Apple Account.

