

- StoreKit
- SKProductsRequestDelegate
-  productsRequest(\_:didReceive:) Deprecated

Instance Method

# productsRequest(\_:didReceive:)

Accepts the App Store response that contains the app-requested product information.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
func productsRequest(
    _ request: SKProductsRequest,
    didReceive response: SKProductsResponse
)
```

**Required**

Deprecated

Get products using Product.products(for:)

## Parameters 

`request`  

The product request sent to the Apple App Store.

`response`  

Detailed information about the list of products.

## See Also

### Related Documentation

In-App Purchase Programming Guide

