

- AppKit
- NSEvent
-  otherEvent(with:location:modifierFlags:timestamp:windowNumber:context:subtype:data1:data2:) 

Type Method

# otherEvent(with:location:modifierFlags:timestamp:windowNumber:context:subtype:data1:data2:)

Creates and returns a new event object that describes a custom event.

macOS

``` source
class func otherEvent(
    with type: NSEvent.EventType,
    location: NSPoint,
    modifierFlags flags: NSEvent.ModifierFlags,
    timestamp time: TimeInterval,
    windowNumber wNum: Int,
    context unusedPassNil: NSGraphicsContext?,
    subtype: Int16,
    data1 d1: Int,
    data2 d2: Int
) -> NSEvent?
```

## Parameters 

`type`  

One of the following event-type constants:

- `NSAppKitDefined`

- `NSSystemDefined`

- `NSApplicationDefined`

- `NSPeriodic`

If `type` is anything else, an `NSInternalInconsistencyException` is raised. Your code should only create events of type `NSApplicationDefined`.

`location`  

The cursor location in the base coordinate system of the window specified by `windowNum`.

`flags`  

An integer bit field containing any of the modifier key masks described in `Getting Unicode Values`, combined using the C bitwise OR operator.

`time`  

The time the event occurred in seconds since system startup.

`wNum`  

An integer that identifies the window device associated with the event, which is associated with the `NSWindow` that will receive the event.

`unusedPassNil`  

The display graphics context of the event. Pass `nil` for this parameter.

`subtype`  

A numeric identifier that further differentiates custom events of types `NSAppKitDefined`, `NSSystemDefined`, and `NSApplicationDefined`. `NSPeriodic` events don’t use this attribute.

`d1`  

Additional data associated with the event. `NSPeriodic` events don’t use these attributes.

`d2`  

Additional data associated with the event. `NSPeriodic` events don’t use these attributes.

## Return Value

The created `NSEvent` object or `nil` if the object couldn’t be created.

## See Also

### Related Documentation

var subtype: NSEvent.EventSubtype

The event’s subtype.

var data1: Int

Additional data associated with this event.

var systemUptime: TimeInterval

The amount of time the system has been awake since the last time it was restarted.

var data2: Int

Additional data associated with this event.

### Creating an event object

class func keyEvent(with: NSEvent.EventType, location: NSPoint, modifierFlags: NSEvent.ModifierFlags, timestamp: TimeInterval, windowNumber: Int, context: NSGraphicsContext?, characters: String, charactersIgnoringModifiers: String, isARepeat: Bool, keyCode: UInt16) -> NSEvent?

Creates and returns a new event object that describes a key event.

class func mouseEvent(with: NSEvent.EventType, location: NSPoint, modifierFlags: NSEvent.ModifierFlags, timestamp: TimeInterval, windowNumber: Int, context: NSGraphicsContext?, eventNumber: Int, clickCount: Int, pressure: Float) -> NSEvent?

Creates and returns a new event object that describes a mouse-down, -up, -moved, or -dragged event.

class func enterExitEvent(with: NSEvent.EventType, location: NSPoint, modifierFlags: NSEvent.ModifierFlags, timestamp: TimeInterval, windowNumber: Int, context: NSGraphicsContext?, eventNumber: Int, trackingNumber: Int, userData: UnsafeMutableRawPointer?) -> NSEvent?

Creates and returns a new event object that describes a tracking-rectangle or cursor-update event.

init?(eventRef: UnsafeRawPointer)

Creates and returns a new event object for a Carbon event.

init?(cgEvent: CGEvent)

Creates and returns an event object for a Core Graphics event.

