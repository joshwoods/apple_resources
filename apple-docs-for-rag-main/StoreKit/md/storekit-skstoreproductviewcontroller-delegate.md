

- StoreKit
- SKStoreProductViewController
-  delegate 

Instance Property

# delegate

The store view controller’s delegate.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+macOS 11.0+

``` source
@MainActor
weak var delegate: (any SKStoreProductViewControllerDelegate)? { get set }
```

## Discussion

Your application must set the delegate before presenting the store view controller.

## See Also

### Related Documentation

In-App Purchase Programming Guide

### Setting a delegate

protocol SKStoreProductViewControllerDelegate

A protocol to call when the customer dismisses the store screen.

