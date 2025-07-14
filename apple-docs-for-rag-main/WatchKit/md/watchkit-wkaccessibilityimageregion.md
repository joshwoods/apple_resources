

- WatchKit
-  WKAccessibilityImageRegion 

Class

# WKAccessibilityImageRegion

An object that defines a portion of an image that you want to call out separately to an assistive app.

watchOS 2.0+

``` source
class WKAccessibilityImageRegion
```

## Overview

The accessibility image region object defines the portion of the image that you want to call out separately and the label you want to apply to that region. Use an accessibility image region object in conjunction with any interface object that displays an image, either as part of its foreground or background content. Register your custom regions using the setAccessibilityImageRegions(_:) method of the corresponding interface object.

## Topics

### Getting the Region Attributes

var frame: CGRect

A portion of the parent image, in the image’s coordinate system.

var label: String

A succinct label that succinctly identifies the purpose of the image region.

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

class WKAlertAction

An object that encapsulates information about a button displayed in an alert or action sheet.

func WKAccessibilityIsVoiceOverRunning() -> Bool

Returns a Boolean value indicating whether VoiceOver is running.

func WKAccessibilityIsReduceMotionEnabled() -> Bool

Returns a Boolean value indicating whether reduced motion is enabled.

