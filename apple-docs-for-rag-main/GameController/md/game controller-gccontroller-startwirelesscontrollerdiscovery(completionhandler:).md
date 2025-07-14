

- Game Controller
- GCController
-  startWirelessControllerDiscovery(completionHandler:) 

Type Method

# startWirelessControllerDiscovery(completionHandler:)

Starts searching for nearby wireless controllers.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class func startWirelessControllerDiscovery(completionHandler: (() -> Void)? = nil)
```

``` source
class func startWirelessControllerDiscovery() async
```

## Parameters 

`completionHandler`  

The block that the framework calls when it completes the request.

## Discussion

Call this method when the user chooses to discover wireless controllers from your interface. The framework searches asynchronously for discoverable wireless controllers. The framework posts the GCControllerDidConnect (Swift) or GCControllerDidConnectNotification (Objective-C) notification when it discovers new controllers. Implement the completion handler you pass to this method to handle when the framework finishes discovering controllers or when it times out.

If you call the startWirelessControllerDiscovery(completionHandler:) method multiple times during discovery, the framework only calls the last completion handler you pass to this method.

## See Also

### Discovering controllers

class func controllers() -> [GCController]

Returns the connected controllers for the device.

class func stopWirelessControllerDiscovery()

Stops searching for nearby wireless controllers.

static let GCControllerDidConnect: NSNotification.Name

A notification that posts after a controller connects to the device.

static let GCControllerDidDisconnect: NSNotification.Name

A notification that posts after a controller disconnects from the device.

