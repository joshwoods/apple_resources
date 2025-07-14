

- UIKit
-  UITableViewRowAction Deprecated

Class

# UITableViewRowAction

A single action to present when the user swipes horizontally in a table row.

iOS 8.0–13.0DeprecatediPadOS 8.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
class UITableViewRowAction
```

Deprecated

Use UISwipeActionsConfiguration instead.

## Overview

Create a UITableViewRowAction object to define a single, custom action for a table row. Users swipe horizontally in a table view to reveal the actions associated with a row. Each row-action object contains the text display, the action to perform, and any specific formatting to apply to that action.

To add custom actions to your table view’s rows, implement the tableView(_:editActionsForRowAt:) method in your table view’s delegate object. In that method, create and return the actions for the indicated row. The table displays your action buttons and executes the appropriate handler block when the user taps one of them.

## Topics

### Creating a table row action

convenience init(style: UITableViewRowAction.Style, title: String?, handler: (UITableViewRowAction, IndexPath) -> Void)

Creates and returns a new table view row action object.

### Configuring the action’s appearance

var style: UITableViewRowAction.Style

The style applied to the action button.

enum Style

Constants that specify the appearance of action buttons.

var title: String?

The title of the action button.

var backgroundColor: UIColor?

The background color of the action button.

var backgroundEffect: UIVisualEffect?

The visual effect to apply to the button.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Row actions

class UISwipeActionsConfiguration

The set of actions to perform when swiping on rows of a table.

class UIContextualAction

An action to display when the user swipes a table row.

