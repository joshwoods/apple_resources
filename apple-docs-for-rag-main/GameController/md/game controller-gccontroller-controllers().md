

- Game Controller
- GCController
-  controllers() 

Type Method

# controllers()

Returns the connected controllers for the device.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class func controllers() -> [GCController]
```

## Return Value

The currently connected controllers.

## Discussion

To track the connection status of controllers, observe the framework notifications. The framework posts the GCControllerDidConnect (Swift) and GCControllerDidBecomeCurrent (Swift) notifications when a controller connects to a device. For Objective-C, it posts the GCControllerDidConnectNotification and GCControllerDidBecomeCurrentNotification notifications. When a controller disconnects from a device, it posts the GCControllerDidDisconnect (Swift) and GCControllerDidStopBeingCurrent (Swift) notifications. For Objective-C, it posts the GCControllerDidDisconnectNotification and GCControllerDidStopBeingCurrentNotification notifications.

## See Also

### Discovering controllers

class func startWirelessControllerDiscovery(completionHandler: (() -> Void)?)

Starts searching for nearby wireless controllers.

class func stopWirelessControllerDiscovery()

Stops searching for nearby wireless controllers.

static let GCControllerDidConnect: NSNotification.Name

A notification that posts after a controller connects to the device.

static let GCControllerDidDisconnect: NSNotification.Name

A notification that posts after a controller disconnects from the device.

