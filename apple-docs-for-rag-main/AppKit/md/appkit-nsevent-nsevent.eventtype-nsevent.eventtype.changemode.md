

- AppKit
- NSEvent
- NSEvent.EventType
-  NSEvent.EventType.changeMode 

Case

# NSEvent.EventType.changeMode

The user changed the mode of a connected device.

macOS 10.15+

``` source
case changeMode
```

## Discussion

In macOS 10.15 and later, you can use an iPad as an additional screen for a macOS device. A double-tap on the side of an Apple Pencil paired with that iPad results in this type of event. AppKit calls the changeMode(with:) method to route these events to the first responder of the key window of the frontmost process.

The object that needs to handle these types of events may not always be the first responder, or be in the active responder chain. To ensure that the events are handled in the right place, call the addLocalMonitorForEvents(matching:handler:) method and handle or redirect the events in your handler block.

## See Also

### Getting Other Input Types

case scrollWheel

The scroll wheel position changed.

