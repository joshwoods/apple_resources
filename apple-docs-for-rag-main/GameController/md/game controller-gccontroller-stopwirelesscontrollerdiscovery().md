

- Game Controller
- GCController
-  stopWirelessControllerDiscovery() 

Type Method

# stopWirelessControllerDiscovery()

Stops searching for nearby wireless controllers.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class func stopWirelessControllerDiscovery()
```

## Discussion

If you call this method while the framework searches for wireless controllers, the framework stops searching and invokes the completion handler you pass to the startWirelessControllerDiscovery(completionHandler:) method.

## See Also

### Discovering controllers

class func controllers() -> [GCController]

Returns the connected controllers for the device.

class func startWirelessControllerDiscovery(completionHandler: (() -> Void)?)

Starts searching for nearby wireless controllers.

static let GCControllerDidConnect: NSNotification.Name

A notification that posts after a controller connects to the device.

static let GCControllerDidDisconnect: NSNotification.Name

A notification that posts after a controller disconnects from the device.

