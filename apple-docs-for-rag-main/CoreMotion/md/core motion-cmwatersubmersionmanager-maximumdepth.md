

- Core Motion
- CMWaterSubmersionManager
-  maximumDepth 

Instance Property

# maximumDepth

The maximum depth supported by the water submersion manager.

iOS 16.0+iPadOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var maximumDepth: Measurement? { get }
```

## Discussion

To access data for dives with a maximum depth of 6 m, add the Shallow Depth and Pressure capability to your app. For more information, see Adding capabilities to your app.

To enable a maximum depth of 40 m, you must apply for the full Submerged Depth and Pressure entitlement. For more information, see Express interest in the Submerged Depth and Pressure API.

