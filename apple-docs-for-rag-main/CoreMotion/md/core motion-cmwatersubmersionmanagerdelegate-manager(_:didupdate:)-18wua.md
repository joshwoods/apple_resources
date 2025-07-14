

- Core Motion
- CMWaterSubmersionManagerDelegate
-  manager(\_:didUpdate:) 

Instance Method

# manager(\_:didUpdate:)

Provides the delegate with updated water temperature data.

iOS 16.0+iPadOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func manager(
    _ manager: CMWaterSubmersionManager,
    didUpdate measurement: CMWaterTemperature
)
```

**Required**

## Parameters 

`manager`  

The manager for water submersion data.

`measurement`  

A data object that contains information about the water temperature and the measurement’s uncertainty.

## Discussion

Implement this method to receive water temperature updates. The system sends temperature updates three times a second while submerged. When on the surface, the system provides updates at a slower rate, and may stop providing updates if the device isn’t moving.

```
nonisolated func manager(_ manager: CMWaterSubmersionManager, didUpdate measurement: CMWaterTemperature) {
    let temp = measurement.temperature
    let uncertainty = measurement.temperatureUncertainty
    let currentTemperature = "\(temp.value) +/- \(uncertainty.value) \(temp.unit)"

    logger.info(("*** \(currentTemperature) ***"))

    Task {
        await myAdd(temperature:measurement)
    }
}
```

## See Also

### Receiving updates

func manager(CMWaterSubmersionManager, didUpdate: CMWaterSubmersionEvent)

Tells the delegate when a water submersion event occurs.

**Required**

func manager(CMWaterSubmersionManager, didUpdate: CMWaterSubmersionMeasurement)

Provides the delegate with a new set of pressure and depth measurements.

**Required**

func manager(CMWaterSubmersionManager, errorOccurred: any Error)

Tells the delegate when an error occurs.

**Required**

