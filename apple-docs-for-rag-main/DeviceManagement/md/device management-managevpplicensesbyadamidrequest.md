

- Device Management
-  ManageVppLicensesByAdamIdRequest 

Object

# ManageVppLicensesByAdamIdRequest

The request to manage licenses.

Device Assignment ServicesVPP License Management

``` source
object ManageVppLicensesByAdamIdRequest
```

## Properties

`adamIdStr`

`string`

 (Required) 

The unique identifier for a product in the iTunes Store.

`associateClientUserIdStrs`

`[string]`

An array of client-user IDs to associate licenses with.

When passing a value for `associateClientUserIdStrs`, you may not also pass a value for `associateSerialNumbers`.

`associateSerialNumbers`

`[string]`

An array of device serial numbers to associate licenses with.

When passing a value for `associateSerialNumbers`, you may not also pass a value for `associateClientUserIdStrs`.

`disassociateClientUserIdStrs`

`[string]`

An array of client-user IDs to disassociate licenses from.

When passing a value for `disassociateClientUserIdStrs`, you may not also pass a value for `disassociateLicenseIdStrs` or `disassociateSerialNumbers`.

`disassociateLicenseIdStrs`

`[string]`

An array of license IDs to disassociate from the user ID or device.

When passing a value for `disassociateLicenseIdStrs`, you may not also pass a value for `disassociateClientUserIdStrs` or `disassociateSerialNumbers`.

`disassociateSerialNumbers`

`[string]`

An array of device serial numbers to disassociate licenses from.

When passing a value for `disassociateSerialNumbers`, you may not also pass a value for `disassociateClientUserIdStrs` or `disassociateLicenseIdStrs`.

`notifyDisassociation`

`boolean`

If `true`, sends notifications when licenses are disassociated. The default is `true`.

`pricingParam`

`string`

The quality of a product in the iTunes Store. The default is `STDQ`. Possible values are:

- `STDQ`: Standard quality

- `PLUS`: High quality

When assigning licenses for books, it is especially important to pass the correct `pricingParam` to the request, so the correct version of the product is assigned. The Get Assets endpoint will return the correct `pricingParam` for the purchased version of the book. If an organization purchases both the standard-quality and high-quality versions of a book, Get Assets will return two records with the same `adamId` but different pricingParams.

`sToken`

`string`

 (Required) 

The authentication token. For more information, see Authentication.

## Discussion

The maximum number of entries allowed in the `associate*` and `disassociate*` arrays are indicated by the `maxBatchAssociateLicenseCount` or `maxBatchDisassociateLicenseCount` fields available from the Service Configuration response.

Requests that exceed the current limits are rejected with the error code 9602 “Invalid Argument” and no work is done. If you receive this error code, query the Service Configuration endpoint to retrieve new `maxBatchAssociateLicenseCount` and `maxBatchDisassociateLicenseCount` values, correct the last request that was rejected, and resend the request.

## See Also

### Request and Response

object ManageVppLicensesByAdamIdResponse

The response from managing licenses.

