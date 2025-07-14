

- UIKit
-  UISwipeActionsConfiguration 

Class

# UISwipeActionsConfiguration

The set of actions to perform when swiping on rows of a table.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UISwipeActionsConfiguration
```

## Overview

Create a UISwipeActionsConfiguration object to associate custom swipe actions with a row of your table view. Users swipe horizontally left or right in a table view to reveal the actions associated with a row. Each swipe-actions object contains the set of actions to display for each type of swipe.

To add custom actions to your table view’s rows, implement the tableView(_:leadingSwipeActionsConfigurationForRowAt:) or tableView(_:trailingSwipeActionsConfigurationForRowAt:) method of your table view’s delegate. In those methods, create and return the actions for the indicated row. The table displays your action buttons and executes the appropriate handler block when the user taps one of them.

## Topics

### Initializing the swipe actions

convenience init(actions: [UIContextualAction])

Creates a swipe action configuration object with the specified set of actions.

### Getting the swipe action information

var actions: [UIContextualAction]

The swipe actions.

var performsFirstActionWithFullSwipe: Bool

A Boolean value indicating whether a full swipe automatically performs the first action.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Row actions

class UIContextualAction

An action to display when the user swipes a table row.

class UITableViewRowAction

A single action to present when the user swipes horizontally in a table row.

Deprecated

