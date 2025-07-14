

- Core Motion
- CMHeadphoneMotionManager
-  startDeviceMotionUpdates(to:withHandler:) 

Instance Method

# startDeviceMotionUpdates(to:withHandler:)

Starts device-motion updates with a handler.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 14.0+watchOS 7.0+

``` source
func startDeviceMotionUpdates(
    to queue: OperationQueue,
    withHandler handler: @escaping CMHeadphoneMotionManager.DeviceMotionHandler
)
```

## Parameters 

`queue`  

The queue for handling updates.

`handler`  

The handler that receives the updates.

## See Also

### Starting and Stopping Updates

func startDeviceMotionUpdates()

Starts device-motion updates.

func startConnectionStatusUpdates()

func stopDeviceMotionUpdates()

Stops device-motion updates.

func stopConnectionStatusUpdates()

