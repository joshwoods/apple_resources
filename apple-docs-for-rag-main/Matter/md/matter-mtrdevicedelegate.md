

- Matter
-  MTRDeviceDelegate 

Protocol

# MTRDeviceDelegate

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.1+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol MTRDeviceDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func device(MTRDevice, receivedAttributeReport: [[String : Any]])

**Required**

func device(MTRDevice, receivedEventReport: [[String : Any]])

**Required**

func device(MTRDevice, stateChanged: MTRDeviceState)

**Required**

func deviceBecameActive(MTRDevice)

func deviceCachePrimed(MTRDevice)

func deviceConfigurationChanged(MTRDevice)

## Relationships

### Inherits From

- NSObjectProtocol

