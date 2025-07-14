

- UIKit
-  UIPress 

Class

# UIPress

An object that represents the presence or movement of a button press on the screen for a particular event.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
class UIPress
```

## Overview

The press specifically encapsulates the pressing of some physically actuated button. All of the press types represent actual physical buttons on one of a variety of remotes. You access UIPress objects through UIEvent objects passed into responder objects for event handling. The gestureRecognizers property returns the gesture recognizers — instances of a concrete subclass of UIGestureRecognizer — that are currently handling the given button press.

## Topics

### Getting a press object’s gesture recognizers

var force: CGFloat

The force of the button press.

var gestureRecognizers: [UIGestureRecognizer]?

The gesture recognizers that are receiving the press.

### Responding to press events

var responder: UIResponder?

A responder object.

### Getting the press’s location

var window: UIWindow?

The window in which the press initially occurred.

### Getting press attributes

var key: UIKey?

The key pressed or released on a physical keyboard.

var type: UIPress.PressType

The type of the specified press.

var phase: UIPress.Phase

The current press phase of the object.

var timestamp: TimeInterval

The time when the press occurred or when it was last mutated.

### Constants

enum Phase

Constants that represent the phases of a button press.

enum PressType

Constants that represent buttons that a person can press.

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

### Button presses

class UIPressesEvent

An event that describes the state of a set of physical buttons that are available to the device, such as those on an associated remote or game controller.

