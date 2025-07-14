

- Apple Pay Web Merchant Registration API
-  Register Merchant 

Web Service Endpoint

# Register Merchant

Register a merchant and its corresponding set of fully qualified domains.

Apple Pay Web Merchant Registration API 1.0+

## URL

``` source
POST https://apple-pay-gateway.apple.com/paymentservices/registerMerchant
```

## HTTP Body

RegisterMerchantRequest

The request body you use to register merchants.

Content-Type: application/json

## Response Codes

` 200 ``OK`

`OK`

Success.

` 400 ``Bad Request`

`Bad Request`

The request is malformed or invalid.

` 401 ``Unauthorized`

`Unauthorized`

The e-commerce platform doesn’t have permission to call this API.

` 417 ``Expectation Failed`

`Expectation Failed`

The e-commerce platform isn’t registered with Apple Developer.

` 500 ``Internal Server Error`

`Internal Server Error`

An internal server error occurred.

## Mentioned in 

Preparing Merchant Domains for Verification

## Discussion

Call this API to register a merchant and their domains. You can register domains in multiple requests. The API has a limit of 99 domain names per `partnerInternalMerchantIdentifier.`

Before making a Register Merchant request, you must prepare each domain included in the request for verification. For more information on domain verification, see Preparing Merchant Domains for Verification.

This request returns no response body for a successful 200 response. Apple Pay servers register the relationship between the e-commerce partner, the merchant, and the merchant’s domains.

Note

To access the sandbox environment, use `POST` `https://apple-pay-gateway-cert.apple.com/paymentservices/registerMerchant`.

## See Also

### Web Merchant Registration

Preparing Merchant Domains for Verification

Host a domain verification file on each domain before requesting registration.

object RegisterMerchantRequest

The request body you use to register merchants.

