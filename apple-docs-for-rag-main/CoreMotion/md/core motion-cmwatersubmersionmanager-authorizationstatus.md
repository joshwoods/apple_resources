

- Core Motion
- CMWaterSubmersionManager
-  authorizationStatus 

Type Property

# authorizationStatus

A value indicating whether the app has user authorization to receive submersion data.

iOS 16.0+iPadOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class var authorizationStatus: CMAuthorizationStatus { get }
```

## Discussion

The system automatically requests authorization to access motion data the first time your app instantiates a `CMWaterSubmersionManager`. You can use this property to check the current authorization status.

## See Also

### Checking availability and authorization

class var waterSubmersionAvailable: Bool

A Boolean value indicating whether the current device supports the submersion manager.

