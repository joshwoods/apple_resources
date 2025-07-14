

- Core Motion
- CMHeadphoneMotionManager
-  CMHeadphoneMotionManager.DeviceMotionHandler 

Type Alias

# CMHeadphoneMotionManager.DeviceMotionHandler

The type of block callback for handling headphone-motion data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+watchOS 2.0+

``` source
typealias DeviceMotionHandler = (CMDeviceMotion?, (any Error)?) -> Void
```

## Discussion

The system calls `CMDeviceMotionHandler` blocks when there is device-motion data to process. You pass the block into startDeviceMotionUpdates(to:withHandler:) as the second argument. Blocks of this type return no value, but take two arguments:

`motion`  
A CMHeadphoneMotionManager object, which encapsulates other objects and a structure representing attitude, rotation rate, gravity, and user acceleration.

`error`  
An error object representing an error when providing gyroscope data. If an error occurs, you should stop gyroscope updates and inform the user of the problem. If there is no error, this argument is `nil`. Core Motion errors are of the CMErrorDomain domain and the CMError type.

## See Also

### Connecting and Disconnecting Headphones

func headphoneMotionManagerDidConnect(CMHeadphoneMotionManager)

Performs a callback to the delegate after you connect headphones.

func headphoneMotionManagerDidDisconnect(CMHeadphoneMotionManager)

Performs a callback to the delegate after you disconnect headphones.

