

- UIKit
- UISwipeActionsConfiguration
-  actions 

Instance Property

# actions

The swipe actions.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var actions: [UIContextualAction] { get }
```

## Discussion

The first object in this array corresponds to the default action, which is the action that’s performed in response to a full swipe.

## See Also

### Getting the swipe action information

var performsFirstActionWithFullSwipe: Bool

A Boolean value indicating whether a full swipe automatically performs the first action.

