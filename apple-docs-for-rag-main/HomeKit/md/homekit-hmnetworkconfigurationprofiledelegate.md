

- HomeKit
-  HMNetworkConfigurationProfileDelegate 

Protocol

# HMNetworkConfigurationProfileDelegate

An interface that your app adopts to receive notifications about changes in the state of network access.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol HMNetworkConfigurationProfileDelegate : NSObjectProtocol
```

## Topics

### Observing network access changes

func profileDidUpdateNetworkAccessMode(HMNetworkConfigurationProfile)

Tells the delegate that the network access mode has changed.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Listening for access changes

var delegate: (any HMNetworkConfigurationProfileDelegate)?

A delegate that HomeKit tells about changes in the state of network access.

