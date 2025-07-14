

- StoreKit
-  SKStoreProductViewControllerDelegate 

Protocol

# SKStoreProductViewControllerDelegate

A protocol to call when the customer dismisses the store screen.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+macOS 11.0+

``` source
protocol SKStoreProductViewControllerDelegate : NSObjectProtocol
```

## Overview

Typically, this protocol is implemented by the view controller in your application that originally displayed the store screen.

## Topics

### Responding to a Dismiss Action

func productViewControllerDidFinish(SKStoreProductViewController)

Called when the user dismisses the store screen.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Setting a delegate

var delegate: (any SKStoreProductViewControllerDelegate)?

The store view controller’s delegate.

