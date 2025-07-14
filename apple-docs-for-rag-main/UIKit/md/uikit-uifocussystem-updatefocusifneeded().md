

- UIKit
- UIFocusSystem
-  updateFocusIfNeeded() 

Instance Method

# updateFocusIfNeeded()

Forces the system to act on a pending focus update for the current environment.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 12.0+visionOS 1.0+

``` source
@MainActor
func updateFocusIfNeeded()
```

## Discussion

If the current environment has a pending focus update, calling this method forces the system to update the focus information immediately instead of waiting for the next run loop cycle. If no focus update is pending, this method does nothing.

You create a pending focus update using the requestFocusUpdate(to:) method. The system may also schedule focus updates in response to interface-related events.

## See Also

### Managing focus updates

func requestFocusUpdate(to: any UIFocusEnvironment)

Submits a request to update the focus state of the specified object.

