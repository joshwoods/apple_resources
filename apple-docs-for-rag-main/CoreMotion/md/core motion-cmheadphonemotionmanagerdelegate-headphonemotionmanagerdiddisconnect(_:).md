

- Core Motion
- CMHeadphoneMotionManagerDelegate
-  headphoneMotionManagerDidDisconnect(\_:) 

Instance Method

# headphoneMotionManagerDidDisconnect(\_:)

Performs a callback to the delegate after you disconnect headphones.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 14.0+watchOS 7.0+

``` source
optional func headphoneMotionManagerDidDisconnect(_ manager: CMHeadphoneMotionManager)
```

## Parameters 

`manager`  

The manager for the disconnected headphones.

## See Also

### Connecting and Disconnecting Headphones

func headphoneMotionManagerDidConnect(CMHeadphoneMotionManager)

Performs a callback to the delegate after you connect headphones.

typealias DeviceMotionHandler

The type of block callback for handling headphone-motion data.

