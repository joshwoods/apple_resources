

- HealthKit
- HKObjectType
-  identifier 

Instance Property

# identifier

A unique string identifying the HealthKit object type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var identifier: String { get }
```

## Discussion

Each object type has a unique identifier. The identifiers can be grouped into different categories: HKQuantityTypeIdentifier, HKCategoryTypeIdentifier, HKCharacteristicTypeIdentifier, HKCorrelationTypeIdentifier, and HKDocumentTypeIdentifier Each group of identifiers is associated with a different concrete subclass of `HKObjectType`.

## See Also

### Getting property data

func requiresPerObjectAuthorization() -> Bool

Returns a Boolean that indicates whether the data type requires per-object authorization.

