

- PassKit (Apple Pay and Wallet)
- PKAddPassesViewController
-  delegate 

Instance Property

# delegate

The view controller’s delegate.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any PKAddPassesViewControllerDelegate)? { get set }
```

## Discussion

For information about the protocol that the delegate must implement, see PKAddPassesViewControllerDelegate.

## See Also

### Adding passes

protocol PKAddPassesViewControllerDelegate

Methods that an add-passes view controller’s delegate implements.

