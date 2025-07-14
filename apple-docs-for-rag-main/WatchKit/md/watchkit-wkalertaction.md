

- WatchKit
-  WKAlertAction 

Class

# WKAlertAction

An object that encapsulates information about a button displayed in an alert or action sheet.

watchOS 2.0+

``` source
class WKAlertAction
```

## Overview

Create instances of this class using the init(title:style:handler:) method and pass them to the presentAlert(withTitle:message:preferredStyle:actions:) method of one of your interface controllers. The sheet uses your action objects to create the corresponding buttons. When creating an alert action, you specify the title and visual style to apply to the button and a block to execute when the button is tapped. Use the defined visual styles to convey the purpose of the button to the user.

## Topics

### Creating an Action

convenience init(title: String, style: WKAlertActionStyle, handler: WKAlertActionHandler)

Creates and returns an action object with the specified button information.

### Constants

enum WKAlertActionStyle

Constants indicating the style of the action button.

typealias WKAlertActionHandler

A block to perform in response to an action.

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

## See Also

### User interface basics

Building watchOS app Interfaces Using the Storyboard

Create the user interface for your watchOS app by nesting stacks.

class WKInterfaceObject

An object that provides information that is common to all interface objects in your watchOS app.

class WKInterfaceController

A class that provides the infrastructure for managing the interface in a watchOS app.

class WKAccessibilityImageRegion

An object that defines a portion of an image that you want to call out separately to an assistive app.

func WKAccessibilityIsVoiceOverRunning() -> Bool

Returns a Boolean value indicating whether VoiceOver is running.

func WKAccessibilityIsReduceMotionEnabled() -> Bool

Returns a Boolean value indicating whether reduced motion is enabled.

