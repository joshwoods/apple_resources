

- HealthKit
- HKQuery
-  objectType 

Instance Property

# objectType

The type of objects being queried.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.2+

``` source
var objectType: HKObjectType? { get }
```

## Discussion

Not all queries return objects of the specified type; however, they all use the object type to filter their results. For example, source queries return a set of data sources that have saved objects with a matching type, while statistics queries return statistical information about the objects with a matching type.

## See Also

### Accessing properties

var predicate: NSPredicate?

A predicate used to filter the objects returned from the HealthKit store.

var sampleType: HKSampleType?

The type of objects being queried.

Deprecated

