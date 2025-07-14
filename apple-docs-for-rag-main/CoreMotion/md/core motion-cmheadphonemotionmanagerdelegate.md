

- Core Motion
-  CMHeadphoneMotionManagerDelegate 

Protocol

# CMHeadphoneMotionManagerDelegate

A set of methods that defines an interface for connecting and disconnecting headphones.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 14.0+watchOS 7.0+

``` source
protocol CMHeadphoneMotionManagerDelegate : NSObjectProtocol
```

## Topics

### Connecting and Disconnecting Headphones

func headphoneMotionManagerDidConnect(CMHeadphoneMotionManager)

Performs a callback to the delegate after you connect headphones.

func headphoneMotionManagerDidDisconnect(CMHeadphoneMotionManager)

Performs a callback to the delegate after you disconnect headphones.

typealias DeviceMotionHandler

The type of block callback for handling headphone-motion data.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Getting the Delegate

var delegate: (any CMHeadphoneMotionManagerDelegate)?

The object that receives headphone motion manager events.

