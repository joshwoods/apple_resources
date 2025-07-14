

- WatchKit
-  WKAccessibilityIsReduceMotionEnabled() 

Function

# WKAccessibilityIsReduceMotionEnabled()

Returns a Boolean value indicating whether reduced motion is enabled.

watchOS 4.0+

``` source
func WKAccessibilityIsReduceMotionEnabled() -> Bool
```

## Discussion

You can use this function to customize your application’s UI when reduced motion is enabled. Note that you can also listen for the WKAccessibilityReduceMotionStatusDidChange (Swift) or WKAccessibilityReduceMotionStatusDidChangeNotification (Objective-C) notification to find out when VoiceOver starts and stops.

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

class WKAccessibilityImageRegion

An object that defines a portion of an image that you want to call out separately to an assistive app.

func WKAccessibilityIsVoiceOverRunning() -> Bool

Returns a Boolean value indicating whether VoiceOver is running.

