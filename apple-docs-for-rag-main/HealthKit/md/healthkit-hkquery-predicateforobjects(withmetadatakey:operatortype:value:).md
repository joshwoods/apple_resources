

- HealthKit
- HKQuery
-  predicateForObjects(withMetadataKey:operatorType:value:) 

Type Method

# predicateForObjects(withMetadataKey:operatorType:value:)

Returns a predicate that matches objects based on the provided metadata key, value, and operator.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func predicateForObjects(
    withMetadataKey key: String,
    operatorType: NSComparisonPredicate.Operator,
    value: Any
) -> NSPredicate
```

## Parameters 

`key`  

The metadata key for the value to be matched. For a list of preset keys, see Metadata Keys. You may also search using custom keys.

`operatorType`  

Defines the relationship used to match the metadata’s value with the provided value.

`value`  

The target value. These values must be NSString, NSNumber, or NSDate instances.

## Return Value

A predicate that matches objects based on the specified metadata key, operator, and value.

## Discussion

Use this convenience method to create a predicate that matches objects based on their metadata, an operator, and a target value. When this predicate is evaluated, it gets the metadata’s value for the provided key. Then the predicate compares that value with the target value using the provided operator.

The following sample uses both the convenience method and a predicate format string to create equivalent predicates.

- Swift
- Objective-C

```
let metadataOperator =
    HKQuery.predicateForObjectsWithMetadataKey(AccuracyCustomMetadataKey,
                                               operatorType: NSPredicateOperatorType.GreaterThanPredicateOperatorType,
                                               value: 75.0)

let explicitMetadataOperator = NSPredicate(format: "%K.%K > %d",
                                           HKPredicateKeyPathMetadata, AccuracyCustomMetadataKey,
                                           75.0)
```

```
NSPredicate *metadataOperator =
    [HKQuery predicateForObjectsWithMetadataKey:AccuracyCustomMetadataKey
                                   operatorType:NSGreaterThanPredicateOperatorType
                                          value:@75.0];

NSPredicate *explicitMetadataOperator =
    [NSPredicate predicateWithFormat:@"%K.%K > %d",
     HKPredicateKeyPathMetadata,
     AccuracyCustomMetadataKey,
     @75.0];
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

class func predicateForObjects(withMetadataKey: String) -> NSPredicate

Returns a predicate that matches any object whose metadata contains the provided key.

class func predicateForObjects(withMetadataKey: String, allowedValues: [Any]) -> NSPredicate

Returns a predicate that matches objects based on the provided metadata key and an array of target values.

class func predicateForObjectsWithNoCorrelation() -> NSPredicate

Returns a predicate that matches all objects that are not associated with a HealthKit correlation.

