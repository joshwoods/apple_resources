

- HealthKit
- HKQuery
-  sampleType Deprecated

Instance Property

# sampleType

The type of objects being queried.

iOS 8.0–9.3DeprecatediPadOS 8.0–9.3DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 13.0+visionOS 1.0–1.0DeprecatedwatchOS 2.0–2.2Deprecated

``` source
var sampleType: HKSampleType? { get }
```

Deprecated

Use objectType instead.

## Discussion

Not all queries return objects of the specified type; however, they all use the object type to generate their results. For example, source queries return a set of data sources that have saved objects with a matching type, while statistics queries return statistical information about the objects with a matching type.

## See Also

### Accessing properties

var predicate: NSPredicate?

A predicate used to filter the objects returned from the HealthKit store.

var objectType: HKObjectType?

The type of objects being queried.

