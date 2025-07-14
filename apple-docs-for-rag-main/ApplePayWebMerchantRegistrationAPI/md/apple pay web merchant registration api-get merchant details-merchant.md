

- Apple Pay Web Merchant Registration API
-  Get Merchant Details 

Web Service Endpoint

# Get Merchant Details

Retrieve information about a registered merchant’s current state by using the merchant’s internal merchant identifier.

Apple Pay Web Merchant Registration API 1.0+

## URL

``` source
GET https://apple-pay-gateway.apple.com/paymentservices/merchant/${partnerInternalMerchantIdentifier}
```

## Path Parameters

`partnerInternalMerchantIdentifier`

`string`

 (Required) 

A unique identifier for the merchant that the e-commerce partner created and used in the Register Merchant request.

Maximum length: `1024`

Value: `/a-zA-Z0-9~-_+&@$!|,.;/`

## Response Codes

` 200 ``OK`

MerchantDetails

`OK`

Success. The response contains an object with information for the registered merchant.

Content-Type: application/json

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

Get information about a merchant you previously registered. You provide the merchant’s unique identifier (`partnerInternalMerchantIdentifier`). A succesful response contains a MerchantDetails object in the response body.

## See Also

### Web Merchant Details

object MerchantDetails

Detailed information for a single registered merchant.

