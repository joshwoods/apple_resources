

- Apple Pay Web Merchant Registration API
-  Unregister Merchant 

Web Service Endpoint

# Unregister Merchant

Unregister one or more domains associated with a previously registered merchant.

Apple Pay Web Merchant Registration API 1.0+

## URL

``` source
POST https://apple-pay-gateway.apple.com/paymentservices/unregisterMerchant
```

## HTTP Body

UnregisterMerchantRequest

The request body for unregistering merchants.

Content-Type: application/json

## Response Codes

` 200 ``OK`

`OK`

Success.

` 400 ``Bad Request`

`Bad Request`

The request is malformed or invalid, or the merchant isn’t registered.

` 401 ``Unauthorized`

`Unauthorized`

The e-commerce platform doesn’t have permission to call this API.

` 417 ``Expectation Failed`

`Expectation Failed`

The e-commerce platform isn’t registered with Apple Developer.

` 500 ``Internal Server Error`

`Internal Server Error`

An internal server error occurred.

## Discussion

Only request to unregister merchants for domains you previously registered using the Register Merchant API.

If you pass a subset of the merchant’s registered domains, Apple Pay server unregisters only those domains and the merchant remains active. If you unregister a merchant’s last-remaining registered domain, Apple Pay servers delete the merchant’s registration.

Note

To access the sandbox environment, use `POST https://apple-pay-gateway-cert.apple.com/paymentservices/unregisterMerchant`.

## See Also

### Web Merchant Unregistration

object UnregisterMerchantRequest

The request body you use to unregister one or more merchant domains.

