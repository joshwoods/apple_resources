

- PassKit (Apple Pay and Wallet)
-  PKAddPassesViewControllerDelegate 

Protocol

# PKAddPassesViewControllerDelegate

Methods that an add-passes view controller’s delegate implements.

iOSiPadOSMac CatalystvisionOS

``` source
protocol PKAddPassesViewControllerDelegate : NSObjectProtocol
```

## Topics

### Delegate methods

func addPassesViewControllerDidFinish(PKAddPassesViewController)

Sent to the delegate after the add-passes view controller has finished.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Adding passes

var delegate: (any PKAddPassesViewControllerDelegate)?

The view controller’s delegate.

