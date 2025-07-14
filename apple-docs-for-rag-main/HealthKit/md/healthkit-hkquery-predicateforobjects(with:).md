

- HealthKit
- HKQuery
-  predicateForObjects(with:) 

Type Method

# predicateForObjects(with:)

Returns a predicate that matches the objects with the specified universally unique identifiers (UUIDs).

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class func predicateForObjects(with UUIDs: Set) -> NSPredicate
```

## Parameters 

`UUIDs`  

The set of UUIDs to be matched.

## Return Value

A predicate that matches the specified objects based on their UUIDs.

## Discussion

HealthKit assigns a UUID to each object when it is saved to the HealthKit store. HealthKit uses these IDs to uniquely identify objects from the store. Use this convenience method to create a predicate that checks an object’s UUID against the provided set of UUIDs. The following sample uses both the convenience method and a predicate format string to create equivalent predicates.

- Swift
- Objective-C

```
let uuids = HKQuery.predicateForObjectsWithUUIDs(myUUIDs)

let explicitUUIDs =
    NSPredicate(format: "%K IN %@", HKPredicateKeyPathUUID, myUUIDs)
```

```
NSPredicate *uuids = [HKQuery predicateForObjectsWithUUIDs:myUUIDs];

NSPredicate *explicitUUIDs = [NSPredicate predicateWithFormat:@"%K IN %@",
                              HKPredicateKeyPathUUID,
                              myUUIDs];
```

## See Also

### Related Documentation

let HKPredicateKeyPathUUID: String

The key path for accessing the object’s UUID inside a predicate format string.

var uuid: UUID

The universally unique identifier (UUID) for this HealthKit object.

### Creating object predicates

class func predicateForObject(with: UUID) -> NSPredicate

Returns a predicate that matches an object with the specified universally unique identifier (UUID).

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

class func predicateForObjectsWithNoCorrelation() -> NSPredicate

Returns a predicate that matches all objects that are not associated with a HealthKit correlation.

