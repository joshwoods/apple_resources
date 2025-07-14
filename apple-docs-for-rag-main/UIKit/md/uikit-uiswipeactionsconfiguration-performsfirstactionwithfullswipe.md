

- UIKit
- UISwipeActionsConfiguration
-  performsFirstActionWithFullSwipe 

Instance Property

# performsFirstActionWithFullSwipe

A Boolean value indicating whether a full swipe automatically performs the first action.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var performsFirstActionWithFullSwipe: Bool { get set }
```

## Discussion

When this property is set to true, a full swipe in the row performs the first action listed in the actions property. The default value of this property is true.

## See Also

### Getting the swipe action information

var actions: [UIContextualAction]

The swipe actions.

