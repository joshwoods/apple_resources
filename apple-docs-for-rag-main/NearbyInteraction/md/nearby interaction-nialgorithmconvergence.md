

- Nearby Interaction
-  NIAlgorithmConvergence 

Class

# NIAlgorithmConvergence

An object that provides the state and reason for user coaching recommendations.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+watchOS 9.0+

``` source
class NIAlgorithmConvergence
```

## Overview

This class conveys the current state of the framework’s Camera Assistance feature when you turn on isCameraAssistanceEnabled. When the status indicates that user action is required to achieve the highest-quality results, instances of this class identify specific actions the user can do to help. To improve the status, the app needs to coach the user such as by presenting instructional text. The information you provide tells the user, for example, where and at what speed to pan the device around the environment.

To listen for the convergence status, implement session(_:didUpdateAlgorithmConvergence:for:).

## Topics

### Determining convergence state

var status: NIAlgorithmConvergenceStatus

The current state of the framework’s Camera Assistance feature.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Camera assistance

Finding devices with precision

Leverage the spatial awareness of ARKit and Apple Ultra Wideband Chips in your app to guide users to a nearby device.

enum NIAlgorithmConvergenceStatus

The possible states of Camera Assistance.

Algorithm Convergence Status

The possible Objective-C states of Camera Assistance.

