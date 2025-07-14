

- Game Controller
- GCMouse
-  mice() 

Type Method

# mice()

Returns any mice that the user connects to the device.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func mice() -> [GCMouse]
```

## Return Value

The currently connected mouse devices.

## See Also

### Discovering mouse devices

static let GCMouseDidConnect: NSNotification.Name

A notification that posts after a mouse connects to the device.

static let GCMouseDidDisconnect: NSNotification.Name

A notification that posts after a mouse disconnects from the device.

