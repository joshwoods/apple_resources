

- AppKit
- NSEvent
-  init(eventRef:) 

Initializer

# init(eventRef:)

Creates and returns a new event object for a Carbon event.

macOS 10.5+

``` source
init?(eventRef: UnsafeRawPointer)
```

## Parameters 

`eventRef`  

The `EventRef` opaque type to be associated with the created `NSEvent` object.

## Return Value

An autoreleased `NSEvent` object corresponding to `eventRef` or `nil` if `eventRef` cannot be converted into an equivalent `NSEvent` object.

## Discussion

This method is valid for all events. The created `NSEvent` object retains the `EventRef` object and is released when the `NSEvent` object is freed.

## See Also

### Related Documentation

var eventRef: UnsafeRawPointer?

An opaque Carbon type associated with this event.

### Creating an event object

class func keyEvent(with: NSEvent.EventType, location: NSPoint, modifierFlags: NSEvent.ModifierFlags, timestamp: TimeInterval, windowNumber: Int, context: NSGraphicsContext?, characters: String, charactersIgnoringModifiers: String, isARepeat: Bool, keyCode: UInt16) -> NSEvent?

Creates and returns a new event object that describes a key event.

class func mouseEvent(with: NSEvent.EventType, location: NSPoint, modifierFlags: NSEvent.ModifierFlags, timestamp: TimeInterval, windowNumber: Int, context: NSGraphicsContext?, eventNumber: Int, clickCount: Int, pressure: Float) -> NSEvent?

Creates and returns a new event object that describes a mouse-down, -up, -moved, or -dragged event.

class func enterExitEvent(with: NSEvent.EventType, location: NSPoint, modifierFlags: NSEvent.ModifierFlags, timestamp: TimeInterval, windowNumber: Int, context: NSGraphicsContext?, eventNumber: Int, trackingNumber: Int, userData: UnsafeMutableRawPointer?) -> NSEvent?

Creates and returns a new event object that describes a tracking-rectangle or cursor-update event.

class func otherEvent(with: NSEvent.EventType, location: NSPoint, modifierFlags: NSEvent.ModifierFlags, timestamp: TimeInterval, windowNumber: Int, context: NSGraphicsContext?, subtype: Int16, data1: Int, data2: Int) -> NSEvent?

Creates and returns a new event object that describes a custom event.

init?(cgEvent: CGEvent)

Creates and returns an event object for a Core Graphics event.

