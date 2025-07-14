

- Safari Services
- SFSafariViewController
-  delegate 

Instance Property

# delegate

An object that provides behavior for the Safari view controller’s Done and Action buttons.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+

``` source
@MainActor
weak var delegate: (any SFSafariViewControllerDelegate)? { get set }
```

## Discussion

Provide a SFSafariViewControllerDelegate object to respond to the Done and Action buttons.

## See Also

### Responding to View Controller Interaction

protocol SFSafariViewControllerDelegate

A protocol used to implement custom event handling for a Safari view controller.

