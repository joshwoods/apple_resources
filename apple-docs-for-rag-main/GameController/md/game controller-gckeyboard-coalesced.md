

- Game Controller
- GCKeyboard
-  coalesced 

Type Property

# coalesced

The keyboard currently connected to the device.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class var coalesced: GCKeyboard? { get }
```

## Discussion

Get the keyboard input values from the keyboard’s keyboardInput controller profile. If the user connects more than one keyboard, the framework represents the combined keyboards with one coalesced keyboard object.

## See Also

### Discovering keyboards

static let GCKeyboardDidConnect: NSNotification.Name

A notification that posts after a keyboard connects to the device.

static let GCKeyboardDidDisconnect: NSNotification.Name

A notification that posts after a single keyboard, or the last of multiple keyboards, disconnects from the device.

