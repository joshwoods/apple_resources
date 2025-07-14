

- Core Motion
-  CMWaterSubmersionManager 

Class

# CMWaterSubmersionManager

An object for managing the collection of pressure and temperature data during submersion.

iOS 16.0+iPadOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class CMWaterSubmersionManager
```

## Mentioned in 

Accessing submersion data

## Overview

Use this class to receive live depth, water pressure, and water temperature data on Apple Watch Ultra.

Start by assigning a usage description using the NSMotionUsageDescription key in your app target’s information property list. You also need to include an entitlement to access the live submersion data.

To access data for dives with a maximum depth of 6 m, add the Shallow Depth and Pressure capability to your app. For more information, see Adding capabilities to your app.

To enable a maximum depth of 40 m, you must apply for the full Submerged Depth and Pressure entitlement. For more information, see Express interest in the Submerged Depth and Pressure API.

Note

As the wearer approaches the maximum depth, the system sends a measurement with an CMWaterSubmersionMeasurement.DepthState.approachingMaxDepth submersion state. When they pass the maximum depth, it sends a CMWaterSubmersionMeasurement.DepthState.pastMaxDepth state, and if they continue to descent past the maximum depth, it sends a CMWaterSubmersionMeasurement.DepthState.sensorDepthError state.

Next, check whether submersion data is available.

```
guard CMWaterSubmersionManager.waterSubmersionAvailable else {
    return false
}
```

If the waterSubmersionAvailable property is true, instantiate a CMWaterSubmersionManager object and assign a delegate.

```
// Instantiate the submersion manager.
submersionManager = CMWaterSubmersionManager()

// Assign the submersion manager delegate.
submersionManager.delegate = self
```

Your delegate then begins receiving updates from the system. For more information, see Accessing submersion data.

## Topics

### Setting the delegate

var delegate: (any CMWaterSubmersionManagerDelegate)?

The object that receives updates about submersion data and events.

### Checking availability and authorization

class var waterSubmersionAvailable: Bool

A Boolean value indicating whether the current device supports the submersion manager.

class var authorizationStatus: CMAuthorizationStatus

A value indicating whether the app has user authorization to receive submersion data.

### Accessing the maximum depth

var maximumDepth: Measurement&lt;UnitLength>?

The maximum depth supported by the water submersion manager.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Water submersion

Accessing submersion data

Use a water-submersion manager to receive water pressure, temperature, and depth data on Apple Watch Ultra.

protocol CMWaterSubmersionManagerDelegate

A delegate that receives updates about ambient pressure, water pressure, water temperature, and submersion events.

class CMWaterSubmersionEvent

An event indicating that the device’s submersion state has changed.

class CMWaterSubmersionMeasurement

An update that contains data about the pressure and depth.

class CMWaterTemperature

An update that contains data about the water temperature.

