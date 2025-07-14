

- Core Motion
- CMWaterSubmersionManager
-  waterSubmersionAvailable 

Type Property

# waterSubmersionAvailable

A Boolean value indicating whether the current device supports the submersion manager.

iOS 16.0+iPadOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class var waterSubmersionAvailable: Bool { get }
```

## Mentioned in 

Accessing submersion data

## Discussion

On Apple Watch Ultra, the system sets `waterSubmersionAvailable` to true. On all other devices and in Simulator, the system sets it to false.

## See Also

### Checking availability and authorization

class var authorizationStatus: CMAuthorizationStatus

A value indicating whether the app has user authorization to receive submersion data.

