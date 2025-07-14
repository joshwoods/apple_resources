

- StoreKit
- SKProductsRequest
-  delegate Deprecated

Instance Property

# delegate

The delegate that receives the response of the app’s products request.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
weak var delegate: (any SKProductsRequestDelegate)? { get set }
```

Deprecated

Use Product.products(for:)

## See Also

### Setting the Delegate

protocol SKProductsRequestDelegate

A set of methods the delegate implements so it receives the product information your app requests.

Deprecated

