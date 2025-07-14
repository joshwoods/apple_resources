

- AppKit
- NSWritingToolsCoordinator
-  view 

Instance Property

# view

The view that currently uses the writing tools coordinator.

macOS 15.2+

``` source
@MainActor
weak var view: NSView? { get }
```

## Discussion

Use this property to refer to the view that currently owns the coordinator object. The system updates this property automatically when you assign the coordinator to the writingToolsCoordinator property of your view. The value of this property is `nil` if there is no associated view.

## See Also

### Managing Writing Tools interactions

var delegate: (any NSWritingToolsCoordinator.Delegate)?

The object that handles Writing Tools interactions for your view.

protocol Delegate

An interface that you use to manage interactions between Writing Tools and your custom text view.

