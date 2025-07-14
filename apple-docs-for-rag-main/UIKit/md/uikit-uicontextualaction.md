

- UIKit
-  UIContextualAction 

Class

# UIContextualAction

An action to display when the user swipes a table row.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIContextualAction
```

## Overview

Create UIContextualAction objects to define the types of actions that can be performed when the user swipes left or right on a table row. Use your actions to initialize a UISwipeActionsConfiguration object in your table view delegate object.

## Topics

### Creating the contextual action

convenience init(style: UIContextualAction.Style, title: String?, handler: UIContextualAction.Handler)

Creates a new contextual action with the specified title and handler.

### Configuring the appearance

var title: String?

The title displayed on the action button.

var backgroundColor: UIColor!

The background color of the action button.

var image: UIImage?

The image to display in the action button.

### Getting the configuration details

var handler: UIContextualAction.Handler

The handler block to execute when the user selects the action.

typealias Handler

The handler block to call in response to the selection of an action.

var style: UIContextualAction.Style

The style that applies to the action button.

enum Style

Constants indicating the style information that applies to the action button.

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

class UISwipeActionsConfiguration

The set of actions to perform when swiping on rows of a table.

class UITableViewRowAction

A single action to present when the user swipes horizontally in a table row.

Deprecated

