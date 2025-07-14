

- HealthKit
- HKQuery
-  predicateForObjects(from:) 

Type Method

# predicateForObjects(from:)

Returns a predicate that matches all the objects that were created by any of the provided source revisions.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class func predicateForObjects(from sourceRevisions: Set) -> NSPredicate
```

## Parameters 

`sourceRevisions`  

A set of source revisions that have saved data to the HealthKit store.

## Return Value

A predicate that matches all the objects created by any of the provided source revisions.

## Discussion

The following sample uses both the convenience method and a predicate format string to create equivalent predicates.

- Swift
- Objective-C

```
let fromSourceRevisions = HKQuery.predicateForObjectsFromSourceRevisions(sourceRevisions)

let explicitFromSourceRevisions = NSPredicate(format: "%K IN %@", HKPredicateKeyPathSourceRevision, sourceRevisions)
```

```
NSPredicate *fromSourceRevisions = [HKQuery predicateForObjectsFromSourceRevisions:sourceRevisions];

NSPredicate *explicitFromSourceRevisions = [NSPredicate predicateWithFormat:@"%K IN %@",
                                            HKPredicateKeyPathSourceRevision,
                                            sourceRevisions];
```

## See Also

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

class func predicateForObjects(withMetadataKey: String) -> NSPredicate

Returns a predicate that matches any object whose metadata contains the provided key.

class func predicateForObjects(withMetadataKey: String, allowedValues: [Any]) -> NSPredicate

Returns a predicate that matches objects based on the provided metadata key and an array of target values.

class func predicateForObjects(withMetadataKey: String, operatorType: NSComparisonPredicate.Operator, value: Any) -> NSPredicate

Returns a predicate that matches objects based on the provided metadata key, value, and operator.

class func predicateForObjectsWithNoCorrelation() -> NSPredicate

Returns a predicate that matches all objects that are not associated with a HealthKit correlation.

