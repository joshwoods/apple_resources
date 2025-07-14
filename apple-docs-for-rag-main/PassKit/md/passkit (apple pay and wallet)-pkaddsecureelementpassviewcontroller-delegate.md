

- PassKit (Apple Pay and Wallet)
- PKAddSecureElementPassViewController
-  delegate 

Instance Property

# delegate

An object that acts as the view controller’s delegate.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any PKAddSecureElementPassViewControllerDelegate)? { get set }
```

## Discussion

The delegate must adopt the PKAddSecureElementPassViewControllerDelegate protocol. The view controller doesn’t retain the delegate.

## See Also

### Responding to the life cycle of a pass

protocol PKAddSecureElementPassViewControllerDelegate

The methods for responding to the life cycle events of a Secure Element pass.

