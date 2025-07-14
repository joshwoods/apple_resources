

- Apple Pay Web Merchant Registration API
-  RegisterMerchantRequest 

Object

# RegisterMerchantRequest

The request body you use to register merchants.

Apple Pay Web Merchant Registration API 1.0+

``` source
object RegisterMerchantRequest
```

## Properties

`domainNames`

`[string]`

 (Required) 

A list of fully qualified domain names for which Apple Pay will process payments for this merchant. Items must be unique. The API is limited to 99 domain names per request.

`encryptTo`

`string`

 (Required) 

The merchant ID associated with the payment processing certificate Apple Pay will use to encrypt payment data on behalf of the merchant you’re registering. Typically, use the merchant ID of the calling e-commerce platform. If the Apple Pay data is decrypted by a party other than the e-commerce platform, use their merchant ID.

`merchantUrl`

`string`

An optional field indicating the website’s top level domain. This domain does not have to be affiliated with the payment transaction nor is it verified. It is used for tracking and debugging.

`partnerInternalMerchantIdentifier`

`string`

 (Required) 

A unique identifier that you create for the merchant you’re registering. Each merchant your e-commerce platform serves must have a unique identifier. This is the same identifier that you pass as the `merchantIdentifier` field into canMakePaymentsWithActiveCard and when requesting and Apple Pay payment session. For more information, see Requesting an Apple Pay payment session.

The `partnerInternalMerchantIdentifier` value must use allowed characters only: `a-zA-Z0-9~-_+&@$!|,.;`

Minimum length: `3`

Maximum length: `1024`

Value: `/ a-zA-Z0-9~-_+&@$!|,.;/`

`partnerMerchantName`

`string`

 (Required) 

A human-readable name for the merchant; the API does not parse this name programmatically.

Maximum length: `1024`

## See Also

### Web Merchant Registration

Preparing Merchant Domains for Verification

Host a domain verification file on each domain before requesting registration.

Register Merchant

Register a merchant and its corresponding set of fully qualified domains.

