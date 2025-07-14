

- WatchKit
-  WKAccessibilityIsVoiceOverRunning() 

Function

# WKAccessibilityIsVoiceOverRunning()

Returns a Boolean value indicating whether VoiceOver is running.

watchOS 2.0+

``` source
func WKAccessibilityIsVoiceOverRunning() -> Bool
```

## Return Value

true if VoiceOver is currently running or false if it is not.

## Discussion

You can use this function to customize your application’s UI specifically for VoiceOver users. For example, you might want UI elements that usually disappear quickly to persist onscreen for VoiceOver users. Note that you can also listen for the WKAccessibilityVoiceOverStatusChanged notification to find out when VoiceOver starts and stops.

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

func WKAccessibilityIsReduceMotionEnabled() -> Bool

Returns a Boolean value indicating whether reduced motion is enabled.

