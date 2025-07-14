

- UIKit
-  UIAlertAction 

Class

# UIAlertAction

An action that can be taken when the user taps a button in an alert.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIAlertAction
```

## Mentioned in 

Getting the user’s attention with alerts and action sheets

## Overview

You use this class to configure information about a single action, including the title to display in the button, any styling information, and a handler to execute when the user taps the button. After creating an alert action object, add it to a UIAlertController object before displaying the corresponding alert to the user.

## Topics

### Creating an alert action

convenience init(title: String?, style: UIAlertAction.Style, handler: ((UIAlertAction) -> Void)?)

Create and return an action with the specified title and behavior.

### Getting the action’s attributes

var title: String?

The title of the action’s button.

var style: UIAlertAction.Style

The style that applies to the action’s button.

var isEnabled: Bool

A Boolean value indicating whether the action is currently enabled.

### Constants

enum Style

Styles to apply to action buttons in an alert.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable
- UIAccessibilityIdentification

## See Also

### Alerts

Getting the user’s attention with alerts and action sheets

Present important information to the user or prompt the user about an important choice.

class UIAlertController

An object that displays an alert message.

