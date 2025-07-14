

- Core Motion
- CMWaterSubmersionManagerDelegate
-  manager(\_:didUpdate:) 

Instance Method

# manager(\_:didUpdate:)

Provides the delegate with a new set of pressure and depth measurements.

iOS 16.0+iPadOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func manager(
    _ manager: CMWaterSubmersionManager,
    didUpdate measurement: CMWaterSubmersionMeasurement
)
```

**Required**

## Parameters 

`manager`  

The manager for water submersion data.

`measurement`  

A data object that contains information about the pressure and depth.

## Discussion

Implement this method to receive updated surface pressure, water pressure, and depth data. The system sends measurement updates three times a second while submerged. When on the surface, the system provides updates at a slower rate, and may stop providing updates if the device isn’t moving.

```
nonisolated func manager(_ manager: CMWaterSubmersionManager, didUpdate measurement: CMWaterSubmersionMeasurement) {

    logger.info("*** Received a depth measurement ***")

    let currentDepth: String
    if let depth = measurement.depth {
        currentDepth = "\(depth.value) \(depth.unit)"
    } else {
        currentDepth = "None"
    }

    let currentSurfacePressure: String
    let surfacePressure = measurement.surfacePressure
    currentSurfacePressure = "\(surfacePressure.value) \(surfacePressure.unit)"

    let currentPressure: String
    if let pressure = measurement.pressure {
        currentPressure = "\(pressure.value) \(pressure.unit)"
    } else {
        currentPressure = "None"
    }

    logger.info("*** Depth: \(currentDepth) ***")
    logger.info("*** Surface Pressure: \(currentSurfacePressure) ***")
    logger.info("*** Pressure: \(currentPressure) ***")

    let submerged: Bool?
    switch measurement.submersionState {
    case .unknown:
        logger.info("*** Unknown Depth ***")
        submerged = nil
    case .notSubmerged:
        logger.info("*** Not Submerged ***")
        submerged = false
    case .submergedShallow:
        logger.info("*** Shallow Depth ***")
        submerged = true
    case .submergedDeep:
        logger.info("*** Deep Depth ***")
        submerged = true
    case .approachingMaxDepth:
        logger.info("*** Approaching Max Depth ***")
        submerged = true
    case .pastMaxDepth:
        logger.info("*** Past Max Depth ***")
        submerged = true
    case .sensorDepthError:
        logger.info("*** A depth error has occurred. ***")
        submerged = nil
    @unknown default:
        fatalError("*** An unknown measurement depth state: \(measurement.submersionState)")
    }

    Task {
        await myAdd(measurement: measurement)
        if let submerged {
            await mySet(submerged: submerged)
        }
    }
}
```

## See Also

### Receiving updates

func manager(CMWaterSubmersionManager, didUpdate: CMWaterSubmersionEvent)

Tells the delegate when a water submersion event occurs.

**Required**

func manager(CMWaterSubmersionManager, didUpdate: CMWaterTemperature)

Provides the delegate with updated water temperature data.

**Required**

func manager(CMWaterSubmersionManager, errorOccurred: any Error)

Tells the delegate when an error occurs.

**Required**

