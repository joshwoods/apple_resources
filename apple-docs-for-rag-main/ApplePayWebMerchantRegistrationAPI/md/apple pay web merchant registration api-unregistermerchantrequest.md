

- Apple Pay Web Merchant Registration API
-  UnregisterMerchantRequest 

Object

# UnregisterMerchantRequest

The request body you use to unregister one or more merchant domains.

Apple Pay Web Merchant Registration API 1.0+

``` source
object UnregisterMerchantRequest
```

## Properties

`domainNames`

`[string]`

 (Required) 

A list of fully qualified domain names to unregister. If a merchant has no remaining domain names after this request removes domains, Apple Pay server deletes the merchant’s registration.

`partnerInternalMerchantIdentifier`

`string`

 (Required) 

A merchant identifier that you create to uniquely identify the registered merchant, and which you use in Apple Pay transactions and in this API.

Maximum length: `1024`

Value: `/a-zA-Z0-9~-_+&@$!|,.;/`

`reason`

`string`

 (Required) 

A short, human-readable phrase that describes the cause of unregistration.

Maximum length: `1024`

## See Also

### Web Merchant Unregistration

Unregister Merchant

Unregister one or more domains associated with a previously registered merchant.

