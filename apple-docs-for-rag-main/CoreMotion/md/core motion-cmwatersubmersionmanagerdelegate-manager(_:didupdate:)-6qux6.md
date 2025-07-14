

- Core Motion
- CMWaterSubmersionManagerDelegate
-  manager(\_:didUpdate:) 

Instance Method

# manager(\_:didUpdate:)

Tells the delegate when a water submersion event occurs.

iOS 16.0+iPadOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func manager(
    _ manager: CMWaterSubmersionManager,
    didUpdate event: CMWaterSubmersionEvent
)
```

**Required**

## Parameters 

`manager`  

The manager for water submersion data.

`event`  

An event indicating that the submersion state has changed.

## Discussion

Implement this method to respond to changes in the device’s submersion state.

```
nonisolated func manager(_ manager: CMWaterSubmersionManager, didUpdate event: CMWaterSubmersionEvent) {

    let submerged: Bool?
    switch event.state {
    case .unknown:
        logger.info("*** Received an unknown event ***")
        submerged = nil

    case .notSubmerged:
        logger.info("*** Not Submerged Event ***")
        submerged = false

    case .submerged:
        logger.info("*** Submerged Event ***")
        submerged = true

    @unknown default:
        fatalError("*** unknown event received: \(event.state) ***")
    }

    Task {
        await myAdd(event: event)
        if let submerged {
            await mySet(submerged: submerged)
        }
    }
}
```

## See Also

### Receiving updates

func manager(CMWaterSubmersionManager, didUpdate: CMWaterSubmersionMeasurement)

Provides the delegate with a new set of pressure and depth measurements.

**Required**

func manager(CMWaterSubmersionManager, didUpdate: CMWaterTemperature)

Provides the delegate with updated water temperature data.

**Required**

func manager(CMWaterSubmersionManager, errorOccurred: any Error)

Tells the delegate when an error occurs.

**Required**

