

- UIKit
- UIWritingToolsCoordinator
-  delegate 

Instance Property

# delegate

The object that handles Writing Tools interactions for your view.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
@MainActor
weak var delegate: (any UIWritingToolsCoordinator.Delegate)? { get }
```

## Discussion

Specify this object at initialization time when creating your `UIWritingToolsCoordinator` object. The object must adopt the UIWritingToolsCoordinator.Delegate protocol, and be capable of modifying your view’s text storage and refreshing the view’s layout and appearance.

## See Also

### Managing Writing Tools interactions

protocol Delegate

An interface that you use to manage interactions between Writing Tools and your custom text view.

