

- HealthKit
- HKQuery
-  predicateForObjects(withMetadataKey:) 

Type Method

# predicateForObjects(withMetadataKey:)

Returns a predicate that matches any object whose metadata contains the provided key.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func predicateForObjects(withMetadataKey key: String) -> NSPredicate
```

## Parameters 

`key`  

The metadata key to match. For a list of preset keys, see Metadata Keys. You may also search for custom keys.

## Return Value

A predicate that matches any object whose metadata contains the provided key.

## Discussion

Use this convenience method to create a predicate that finds all objects with a specific key stored in their metadata. The following sample uses both the convenience method and a predicate format string to create equivalent predicates.

- Swift
- Objective-C

```
let metadataKey = HKQuery.predicateForObjectsWithMetadataKey(HKMetadataKeyFoodType)

let explicitMetadataKey =
    NSPredicate(format: "%K.%K != nil",
                HKPredicateKeyPathMetadata, HKMetadataKeyFoodType)
```

```
NSPredicate *metadataKey =
    [HKQuery predicateForObjectsWithMetadataKey:HKMetadataKeyFoodType];

NSPredicate *explicitMetadataKey =
    [NSPredicate predicateWithFormat:@"%K.%K != nil",
     HKPredicateKeyPathMetadata,
     HKMetadataKeyFoodType];
```

## See Also

### Related Documentation

let HKPredicateKeyPathMetadata: String

The key path for accessing the object’s metadata dictionary inside a predicate format string.

var metadata: [String : Any]?

The metadata for this HealthKit object.

### Creating object predicates

class func predicateForObject(with: UUID) -> NSPredicate

Returns a predicate that matches an object with the specified universally unique identifier (UUID).

class func predicateForObjects(with: Set&lt;UUID>) -> NSPredicate

Returns a predicate that matches the objects with the specified universally unique identifiers (UUIDs).

class func predicateForObjects(from: HKSource) -> NSPredicate

Returns a predicate that matches all the objects that were created by the provided source.

class func predicateForObjects(from: Set&lt;HKSource>) -> NSPredicate

Returns a predicate that matches all the objects that were created by any of the provided sources.

class func predicateForObjects(from: Set&lt;HKDevice>) -> NSPredicate

Returns a predicate that matches all the objects that were created by any of the provided devices.

class func predicateForObjects(withDeviceProperty: String, allowedValues: Set&lt;String>) -> NSPredicate

Returns a predicate that matches all objects created by devices with the specified properties.

class func predicateForObjects(from: Set&lt;HKSourceRevision>) -> NSPredicate

Returns a predicate that matches all the objects that were created by any of the provided source revisions.

class func predicateForObjects(withMetadataKey: String, allowedValues: [Any]) -> NSPredicate

Returns a predicate that matches objects based on the provided metadata key and an array of target values.

class func predicateForObjects(withMetadataKey: String, operatorType: NSComparisonPredicate.Operator, value: Any) -> NSPredicate

Returns a predicate that matches objects based on the provided metadata key, value, and operator.

class func predicateForObjectsWithNoCorrelation() -> NSPredicate

Returns a predicate that matches all objects that are not associated with a HealthKit correlation.

