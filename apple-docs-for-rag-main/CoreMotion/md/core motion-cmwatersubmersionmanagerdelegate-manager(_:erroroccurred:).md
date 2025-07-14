

- Core Motion
- CMWaterSubmersionManagerDelegate
-  manager(\_:errorOccurred:) 

Instance Method

# manager(\_:errorOccurred:)

Tells the delegate when an error occurs.

iOS 16.0+iPadOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func manager(
    _ manager: CMWaterSubmersionManager,
    errorOccurred error: any Error
)
```

**Required**

## Parameters 

`manager`  

The manager for water submersion data.

`error`  

An error object that contains information about the error.

## Mentioned in 

Accessing submersion data

## Discussion

Implement this method to respond to errors.

```
// Respond to errors.
nonisolated func manager(_ manager: CMWaterSubmersionManager, errorOccurred error: Error) {
    logger.error("*** An error occurred: \(error.localizedDescription) ***")
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

func manager(CMWaterSubmersionManager, didUpdate: CMWaterTemperature)

Provides the delegate with updated water temperature data.

**Required**

