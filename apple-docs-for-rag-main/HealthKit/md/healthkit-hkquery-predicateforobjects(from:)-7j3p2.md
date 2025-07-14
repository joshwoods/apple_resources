

- HealthKit
- HKQuery
-  predicateForObjects(from:) 

Type Method

# predicateForObjects(from:)

Returns a predicate that matches all the objects that were created by the provided source.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func predicateForObjects(from source: HKSource) -> NSPredicate
```

## Parameters 

`source`  

The source that saved data into the HealthKit store. The source object represents either an app or a devices capable of saving data directly into the HealthKit store (for example, a linked Bluetooth heart rate monitor).

## Return Value

A predicate that matches all the objects created by the provided source.

## Discussion

Use this convenience method to create a predicate that finds all the objects from a specific app or device. The following sample uses both the convenience method and a predicate format string to create equivalent predicates.

- Swift
- Objective-C

```
let fromSource = HKQuery.predicateForObjectsFromSource(source)

let explicitFromSource =
    NSPredicate(format: "%K == %@", HKPredicateKeyPathSource, source)
```

```
NSPredicate *fromSource = [HKQuery predicateForObjectsFromSource:source];

NSPredicate *explicitFromSource = [NSPredicate predicateWithFormat:@"%K == %@",
                                   HKPredicateKeyPathSource,
                                   source];
```

## See Also

### Related Documentation

var source: HKSource

A HealthKit source, representing the app or device that created this object.

Deprecated

class HKSourceQuery

A query that returns a list of sources, such as apps and devices, that have saved matching queries to the HealthKit store.

### Creating object predicates

class func predicateForObject(with: UUID) -> NSPredicate

Returns a predicate that matches an object with the specified universally unique identifier (UUID).

class func predicateForObjects(with: Set&lt;UUID>) -> NSPredicate

Returns a predicate that matches the objects with the specified universally unique identifiers (UUIDs).

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

class func predicateForObjectsWithNoCorrelation() -> NSPredicate

Returns a predicate that matches all objects that are not associated with a HealthKit correlation.

