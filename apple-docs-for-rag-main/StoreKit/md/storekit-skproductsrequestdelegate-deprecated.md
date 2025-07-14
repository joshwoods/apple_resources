

- StoreKit
-  SKProductsRequestDelegate Deprecated

Protocol

# SKProductsRequestDelegate

A set of methods the delegate implements so it receives the product information your app requests.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
protocol SKProductsRequestDelegate : SKRequestDelegate
```

Deprecated

Get products using Product.products(for:)

## Mentioned in 

Fetching product information from the App Store

## Overview

The SKProductsRequestDelegate protocol declares methods that are implemented by the delegate of an SKProductsRequest object. The delegate receives the product information that the product request referred to. Your app uses this information when presenting products to users in its in-app store.

Warning

Responses received by the `SKProductsRequestDelegate` may not be returned on a specific thread. If you make assumptions about which queue will handle delegate responses, you may encounter unintended performance and compatibility issues in the future.

## Topics

### Receiving the Response

func productsRequest(SKProductsRequest, didReceive: SKProductsResponse)

Accepts the App Store response that contains the app-requested product information.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- SKRequestDelegate

## See Also

### Setting the Delegate

var delegate: (any SKProductsRequestDelegate)?

The delegate that receives the response of the app’s products request.

Deprecated

