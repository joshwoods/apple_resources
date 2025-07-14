

- AppKit
- NSWritingToolsCoordinator
-  stopWritingTools() 

Instance Method

# stopWritingTools()

Stops the current Writing Tools operation and dismisses the system UI.

macOS 15.2+

``` source
@MainActor
func stopWritingTools()
```

## Discussion

Call this method to abort the current Writing Tools operation. This method dismisses the system’s Writing Tools UI and stops any in-flight interactions with your view. This method does not undo any changes that Writing Tools already made to your view’s content.

## See Also

### Managing the current state

var state: NSWritingToolsCoordinator.State

The current level of Writing Tools activity in your view.

enum State

The states that indicate the current activity, if any, Writing Tools is performing in your view.

