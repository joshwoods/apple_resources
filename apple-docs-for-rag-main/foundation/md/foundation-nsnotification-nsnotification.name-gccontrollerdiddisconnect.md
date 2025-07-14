

- Foundation
- NSNotification
- NSNotification.Name
-  GCControllerDidDisconnect 

Type Property

# GCControllerDidDisconnect

A notification that posts after a controller disconnects from the device.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
static let GCControllerDidDisconnect: NSNotification.Name
```

## Discussion

The notification object is the GCController object that disconnects from the device.

## See Also

### Game Controller

static let GCControllerDidConnect: NSNotification.Name

A notification that posts after a controller connects to the device.

static let GCControllerDidBecomeCurrent: NSNotification.Name

A notification that posts when a controller becomes the current controller.

static let GCControllerDidStopBeingCurrent: NSNotification.Name

A notification that posts when a controller stops being the current controller.

static let GCControllerUserCustomizationsDidChange: NSNotification.Name

A notification that posts when the user customizes the button mappings or other settings of a controller.

static let GCKeyboardDidConnect: NSNotification.Name

A notification that posts after a keyboard connects to the device.

static let GCKeyboardDidDisconnect: NSNotification.Name

A notification that posts after a single keyboard, or the last of multiple keyboards, disconnects from the device.

static let GCMouseDidBecomeCurrent: NSNotification.Name

A notification that posts when a mouse becomes the most recent mouse that the user connects.

static let GCMouseDidConnect: NSNotification.Name

A notification that posts after a mouse connects to the device.

static let GCMouseDidDisconnect: NSNotification.Name

A notification that posts after a mouse disconnects from the device.

static let GCMouseDidStopBeingCurrent: NSNotification.Name

A notification that posts when a mouse stops being the most recent mouse that the user connects.

static let GCRacingWheelDidConnect: NSNotification.Name

A notification that posts after a racing wheel controller connects to the device.

static let GCRacingWheelDidDisconnect: NSNotification.Name

A notification that posts after a racing wheel controller disconnects from the device.

