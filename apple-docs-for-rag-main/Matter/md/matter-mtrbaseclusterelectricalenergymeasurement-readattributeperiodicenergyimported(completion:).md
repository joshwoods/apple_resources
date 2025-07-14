

- Matter
- MTRBaseClusterElectricalEnergyMeasurement
-  readAttributePeriodicEnergyImported(completion:) 

Instance Method

# readAttributePeriodicEnergyImported(completion:)

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
func readAttributePeriodicEnergyImported(completion: @escaping (MTRElectricalEnergyMeasurementClusterEnergyMeasurementStruct?, (any Error)?) -> Void)
```

``` source
func readAttributePeriodicEnergyImported() async throws -> MTRElectricalEnergyMeasurementClusterEnergyMeasurementStruct
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func readAttributePeriodicEnergyImported() async throws -> MTRElectricalEnergyMeasurementClusterEnergyMeasurementStruct
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

