

- Matter
- MTRBaseClusterElectricalEnergyMeasurement
-  subscribeAttributePeriodicEnergyImported(with:subscriptionEstablished:reportHandler:) 

Instance Method

# subscribeAttributePeriodicEnergyImported(with:subscriptionEstablished:reportHandler:)

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
func subscribeAttributePeriodicEnergyImported(
    with params: MTRSubscribeParams,
    subscriptionEstablished: MTRSubscriptionEstablishedHandler?,
    reportHandler: @escaping (MTRElectricalEnergyMeasurementClusterEnergyMeasurementStruct?, (any Error)?) -> Void
)
```

