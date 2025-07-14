

- Game Controller
- GCDevice
-  physicalInputProfile Deprecated

Instance Property

# physicalInputProfile

The device’s physical input profile, such as a controller’s extended gamepad.

iOS 14.0–16.0DeprecatediPadOS 14.0–16.0DeprecatedMac Catalyst 14.0–16.0DeprecatedmacOS 11.0–13.0DeprecatedtvOS 14.0–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var physicalInputProfile: GCPhysicalInputProfile { get }
```

**Required**

Deprecated

Use the physicalInputProfile property on GCController instead. For GCKeyboard, use the keyboardInput property. For GCMouse, use the mouseInput property.

## See Also

### Handling input

var handlerQueue: dispatch_queue_t

The dispatch queue that the framework uses to call element value change handlers.

**Required**

