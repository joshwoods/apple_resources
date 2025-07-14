

- CarPlay
-  CPAlertAction 

Class

# CPAlertAction

An object that encapsulates an action the user can perform on an action sheet or alert.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPAlertAction
```

## Overview

Use an alert action to display a button on an alert. The combination of the alert and the action styles determines the appearance of the action button. To perform an action after the user taps the button, provide a block to the action’s handler property.

## Topics

### Creating an Alert Action

init(title: String, style: CPAlertAction.Style, handler: CPAlertActionHandler)

Creates an alert action with a title, style, and action handler.

### Getting the Title

var title: String

The action button’s title.

### Getting the Action Style

var style: CPAlertAction.Style

The display style for the action button.

enum Style

Display styles for an alert’s action button.

### Getting the Action Handler

var handler: CPAlertActionHandler

The closure that CarPlay invokes after the user taps the action button.

typealias CPAlertActionHandler

The declaration for an alert action handler.

### Initializers

init(title: String, color: UIColor, handler: CPAlertActionHandler)

### Instance Properties

var color: UIColor?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Actions and Alerts

class CPActionSheetTemplate

A template that displays a modal action sheet.

class CPAlertTemplate

A template that displays a modal alert.

