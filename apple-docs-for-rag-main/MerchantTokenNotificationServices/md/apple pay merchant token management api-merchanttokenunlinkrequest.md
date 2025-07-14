

- Apple Pay Merchant Token Management API
-  MerchantTokenUnlinkRequest 

Object

# MerchantTokenUnlinkRequest

The request body you use to invalidate a merchant token.

App Store Connect API 1.0+

``` source
object MerchantTokenUnlinkRequest
```

## Properties

`merchantTokenIdentifier`

`string`

 (Required) 

The merchant token identifier to invalidate.

Maximum length: `64`

## See Also

### Merchant token invalidation

Invalidate a Merchant Token

Invalidate a merchant token associated with your merchant identifier, making it invalid for future transaction authorizations.

