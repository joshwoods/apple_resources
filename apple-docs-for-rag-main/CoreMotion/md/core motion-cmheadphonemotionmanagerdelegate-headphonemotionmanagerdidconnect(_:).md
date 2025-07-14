

- Core Motion
- CMHeadphoneMotionManagerDelegate
-  headphoneMotionManagerDidConnect(\_:) 

Instance Method

# headphoneMotionManagerDidConnect(\_:)

Performs a callback to the delegate after you connect headphones.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 14.0+watchOS 7.0+

``` source
optional func headphoneMotionManagerDidConnect(_ manager: CMHeadphoneMotionManager)
```

## Parameters 

`manager`  

The manager for the connected headphones.

## See Also

### Connecting and Disconnecting Headphones

func headphoneMotionManagerDidDisconnect(CMHeadphoneMotionManager)

Performs a callback to the delegate after you disconnect headphones.

typealias DeviceMotionHandler

The type of block callback for handling headphone-motion data.

