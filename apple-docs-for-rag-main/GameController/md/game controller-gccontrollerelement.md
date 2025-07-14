

- Game Controller
-  GCControllerElement 

Class

# GCControllerElement

An input for a physical control, such as a button or thumbstick.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class GCControllerElement
```

## Overview

`GCControllerElement` is an abstract superclass for specific types of elements that represent controls on a game controller. Use the respective subclasses to either get the input of an element directly or set a handler that the element calls when the user changes a value. This class provides support for common features.

For complex elements that have subelements, you can get the containing element using the collection property. For example, a direction pad (GCControllerDirectionPad) has two axis control and four button subelements.

If the user binds a controller element to a system gesture, the system sends the input to the system gesture recognizer first. If it doesn’t recognize a gesture, the system sends the input to your app but with a delay. If it does recognize a gesture, it doesn’t send any input to your app.

To change this default behavior, you can set the preferredSystemGestureState property to GCControllerElement.SystemGestureState.alwaysReceive to receive the input simultaneously without delay. Alternatively, set it to GCControllerElement.SystemGestureState.disabled to disable the system gesture and receive the input exclusively. Use the isBoundToSystemGesture property to check whether the user included an element in a system gesture.

Use the isAnalog property to determine whether an element’s input value is a range of values or a discrete digital value.

## Topics

### Accessing input values

var isAnalog: Bool

A Boolean value that indicates whether the element provides analog data.

### Getting a localized name

var localizedName: String?

The localized name for the element or the remapped element.

var unmappedLocalizedName: String?

The element’s localized name, not the remapped name.

### Displaying a symbol

var sfSymbolsName: String?

A system symbol for the element or the remapped element.

var unmappedSfSymbolsName: String?

The element’s system symbol, not the remapped symbol.

### Accessing elements by key

var aliases: Set&lt;String>

The element’s aliases you use when accessing it with the subscript notation.

### Getting the containing element

var collection: GCControllerElement?

The enclosing element for this element.

### Handling system gesture input

var isBoundToSystemGesture: Bool

A Boolean value that indicates whether the user binds the element to a system gesture.

var preferredSystemGestureState: GCControllerElement.SystemGestureState

The preferred state for handling input when the user binds the element to a system gesture.

enum SystemGestureState

A state for handling input when an element is part of a system gesture.

## Relationships

### Inherits From

- NSObject

### Inherited By

- GCControllerAxisInput
- GCControllerButtonInput
- GCControllerDirectionPad
- GCControllerTouchpad

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Accessing controller elements

class GCControllerAxisInput

A control element that tracks movement along an axis.

class GCControllerButtonInput

A control element that represents a button touch or press.

class GCControllerTouchpad

A control element that represents a touch event on a touchpad.

class GCControllerDirectionPad

A control element associated with a directional pad or a thumbstick.

class GCDeviceCursor

A control element for the cursor used as a directional pad.

class GCDualSenseAdaptiveTrigger

A class that encapsulates the features of a DualSense adaptive trigger.

