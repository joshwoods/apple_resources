

- External Accessory
-  EAAccessoryDelegate 

Protocol

# EAAccessoryDelegate

A protocol that defines an optional method for receiving notifications when the associated accessory object is disconnected.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.0+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
protocol EAAccessoryDelegate : NSObjectProtocol
```

## Topics

### Responding to Disconnection Events

func accessoryDidDisconnect(EAAccessory)

Tells the delegate that the specified accessory was disconnected from the device.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to Disconnection Events

var delegate: (any EAAccessoryDelegate)?

The object that acts as the delegate of the accessory.

