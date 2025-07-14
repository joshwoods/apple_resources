

- Core Location
- CLLocationSourceInformation
-  isSimulatedBySoftware 

Instance Property

# isSimulatedBySoftware

A Boolean value that indicates whether the system generates the location using on-device software simulation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var isSimulatedBySoftware: Bool { get }
```

## Discussion

Core Location sets isSimulatedBySoftware to `true` if the system generated the location using on-device software simulation. You can simulate locations by loading GPX files using the Xcode debugger. The default value is `false`.

## See Also

### Identifying the source of location data

var isProducedByAccessory: Bool

A Boolean value that indicates whether the system receives the location from an external accessory.

