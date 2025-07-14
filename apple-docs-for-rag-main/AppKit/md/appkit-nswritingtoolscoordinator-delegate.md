

- AppKit
- NSWritingToolsCoordinator
-  delegate 

Instance Property

# delegate

The object that handles Writing Tools interactions for your view.

macOS 15.2+

``` source
@MainActor
weak var delegate: (any NSWritingToolsCoordinator.Delegate)? { get }
```

## Discussion

Specify this object at initialization time when creating your `NSWritingToolsCoordinator` object. The object must adopt the NSWritingToolsCoordinator.Delegate protocol, and be capable of modifying your view’s text storage and refreshing the view’s layout and appearance.

## See Also

### Managing Writing Tools interactions

protocol Delegate

An interface that you use to manage interactions between Writing Tools and your custom text view.

var view: NSView?

The view that currently uses the writing tools coordinator.

