

- Core Motion
- CMHeadphoneMotionManager
-  startDeviceMotionUpdates() 

Instance Method

# startDeviceMotionUpdates()

Starts device-motion updates.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 14.0+watchOS 7.0+

``` source
func startDeviceMotionUpdates()
```

## Discussion

To receive the latest device-motion data, examine the deviceMotion property.

## See Also

### Starting and Stopping Updates

func startDeviceMotionUpdates(to: OperationQueue, withHandler: CMHeadphoneMotionManager.DeviceMotionHandler)

Starts device-motion updates with a handler.

func startConnectionStatusUpdates()

func stopDeviceMotionUpdates()

Stops device-motion updates.

func stopConnectionStatusUpdates()

