

- PassKit (Apple Pay and Wallet)
-  PKAddSecureElementPassViewControllerDelegate 

Protocol

# PKAddSecureElementPassViewControllerDelegate

The methods for responding to the life cycle events of a Secure Element pass.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
protocol PKAddSecureElementPassViewControllerDelegate : NSObjectProtocol
```

## Topics

### Responding to pass addition

func addSecureElementPassViewController(PKAddSecureElementPassViewController, didFinishAddingSecureElementPasses: [PKSecureElementPass]?, error: (any Error)?)

Tells the delegate when PassKit finishes adding one or more Secure Element passes.

**Required**

func addSecureElementPassViewController(PKAddSecureElementPassViewController, didFinishAdding: PKSecureElementPass?, error: (any Error)?)

Tells the delegate when PassKit finishes adding a Secure Element pass.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to the life cycle of a pass

var delegate: (any PKAddSecureElementPassViewControllerDelegate)?

An object that acts as the view controller’s delegate.

