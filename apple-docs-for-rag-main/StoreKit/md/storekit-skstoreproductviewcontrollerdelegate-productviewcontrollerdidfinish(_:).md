

- StoreKit
- SKStoreProductViewControllerDelegate
-  productViewControllerDidFinish(\_:) 

Instance Method

# productViewControllerDidFinish(\_:)

Called when the user dismisses the store screen.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+macOS 11.0+

``` source
optional func productViewControllerDidFinish(_ viewController: SKStoreProductViewController)
```

## Parameters 

`viewController`  

The store view controller whose interface was dismissed by the user.

## Discussion

Your delegate should call the dismissModalViewControllerAnimated: method on the view controller that originally presented the store screen. If your app paused any other activities before presenting the store, it can restart those services in this method.

## See Also

### Related Documentation

In-App Purchase Programming Guide

