

- AppKit
- NSWritingToolsCoordinator
-  state 

Instance Property

# state

The current level of Writing Tools activity in your view.

macOS 15.2+

``` source
@MainActor
var state: NSWritingToolsCoordinator.State { get }
```

## Discussion

Use this property to determine when Writing Tools is actively making changes to your view. During the course of Writing Tools interactions, the system reports state changes to the delegate’s writingToolsCoordinator(_:willChangeTo:completion:) method and updates this property accordingly.

## See Also

### Managing the current state

func stopWritingTools()

Stops the current Writing Tools operation and dismisses the system UI.

enum State

The states that indicate the current activity, if any, Writing Tools is performing in your view.

