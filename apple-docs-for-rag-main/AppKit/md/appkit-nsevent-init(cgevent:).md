

- AppKit
- NSEvent
-  init(cgEvent:) 

Initializer

# init(cgEvent:)

Creates and returns an event object for a Core Graphics event.

macOS 10.5+

``` source
init?(cgEvent: CGEvent)
```

## Parameters 

`cgEvent`  

A CGEvent opaque type that represents an event.

## Return Value

An autoreleased `NSEvent` object that is equivalent to `cgEvent`.

## Discussion

The returned object retains the `CGEventRef` object (`cgEvent`) until it (the Objective-C object) is freed—it then releases the `CGEventRef` object. If no Cocoa event corresponds to the `CGEventRef` object, this method returns `nil`.

## See Also

### Related Documentation

var cgEvent: CGEvent?

The Core Graphics event object corresponding to this event.

### Creating an event object

class func keyEvent(with: NSEvent.EventType, location: NSPoint, modifierFlags: NSEvent.ModifierFlags, timestamp: TimeInterval, windowNumber: Int, context: NSGraphicsContext?, characters: String, charactersIgnoringModifiers: String, isARepeat: Bool, keyCode: UInt16) -> NSEvent?

Creates and returns a new event object that describes a key event.

class func mouseEvent(with: NSEvent.EventType, location: NSPoint, modifierFlags: NSEvent.ModifierFlags, timestamp: TimeInterval, windowNumber: Int, context: NSGraphicsContext?, eventNumber: Int, clickCount: Int, pressure: Float) -> NSEvent?

Creates and returns a new event object that describes a mouse-down, -up, -moved, or -dragged event.

class func enterExitEvent(with: NSEvent.EventType, location: NSPoint, modifierFlags: NSEvent.ModifierFlags, timestamp: TimeInterval, windowNumber: Int, context: NSGraphicsContext?, eventNumber: Int, trackingNumber: Int, userData: UnsafeMutableRawPointer?) -> NSEvent?

Creates and returns a new event object that describes a tracking-rectangle or cursor-update event.

class func otherEvent(with: NSEvent.EventType, location: NSPoint, modifierFlags: NSEvent.ModifierFlags, timestamp: TimeInterval, windowNumber: Int, context: NSGraphicsContext?, subtype: Int16, data1: Int, data2: Int) -> NSEvent?

Creates and returns a new event object that describes a custom event.

init?(eventRef: UnsafeRawPointer)

Creates and returns a new event object for a Carbon event.

