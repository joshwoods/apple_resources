

- HealthKit
- HKQuery
-  predicateForObjectsWithNoCorrelation() 

Type Method

# predicateForObjectsWithNoCorrelation()

Returns a predicate that matches all objects that are not associated with a HealthKit correlation.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func predicateForObjectsWithNoCorrelation() -> NSPredicate
```

## Return Value

A predicate that matches all objects that are not associated with any HealthKit correlations.

## Discussion

Use this convenience method to create a predicate that matches all objects not associated with a HKCorrelation object. The following sample uses both the convenience method and a predicate format string to create equivalent predicates.

- Swift
- Objective-C

```
let noncorrelated = HKQuery.predicateForObjectsWithNoCorrelation()

let explicitNoncorrelated =
    NSPredicate(format: "%K == nil", HKPredicateKeyPathCorrelation)
```

```
NSPredicate *noncorrelated = [HKQuery predicateForObjectsWithNoCorrelation];

NSPredicate *explicitNoncorrelated =
[NSPredicate predicateWithFormat:@"%K == nil", HKPredicateKeyPathCorrelation];
```

## See Also

### Related Documentation

let HKPredicateKeyPathCorrelation: String

The key path for accessing the object’s correlation inside a predicate format string.

class HKCorrelation

A sample that groups multiple related samples into a single entry.

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

class func predicateForObjects(withMetadataKey: String, operatorType: NSComparisonPredicate.Operator, value: Any) -> NSPredicate

Returns a predicate that matches objects based on the provided metadata key, value, and operator.

