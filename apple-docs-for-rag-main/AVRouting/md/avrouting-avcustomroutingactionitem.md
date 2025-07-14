

- AVRouting
-  AVCustomRoutingActionItem 

Class

# AVCustomRoutingActionItem

An object that represents a custom action item to display in a device route picker.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
class AVCustomRoutingActionItem
```

## Overview

Use this class to specify supplemental action items to display in the list of discovered routes. Tapping a custom item dismisses the picker and calls the customRoutingController(_:didSelect:) method of AVCustomRoutingControllerDelegate.

## Topics

### Configuring an item

var type: UTType

A type with an identifier that matches a value in the app’s configuration.

var overrideTitle: String?

A string to use to override the title of the item’s type.

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

### Media routing

class AVCustomRoutingController

An object that manages the connection from a device to a destination.

protocol AVCustomRoutingControllerDelegate

A protocol for delegates of a custom routing controller.

class AVCustomRoutingEvent

An object that represents an event that occurs on a route.

