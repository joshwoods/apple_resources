

- AppKit
- NSTableView
-  rowActionsVisible 

Instance Property

# rowActionsVisible

A Boolean value indicating whether a table row’s actions are visible.

macOS 10.11+

``` source
@MainActor
var rowActionsVisible: Bool { get set }
```

## Discussion

This property contains a Boolean value indicating whether a table row’s actions are visible or not—the user has swiped the row to reveal the row actions. Set the value of this property to false to hide any visible row actions. Setting the value of this property to true is not supported, and will result in an exception.

