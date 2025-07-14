

- HealthKit
- HKVerifiableClinicalRecordQueryDescriptor
-  predicate 

Instance Property

# predicate

A predicate that limits the results returned by the query.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOS

``` source
var predicate: NSPredicate?
```

## Discussion

If this property is `nil`, the query returns all records of the specified type.

## See Also

### Accessing Query Properties

var recordTypes: [HKVerifiableClinicalRecordCredentialType]

The types of records returned by this query.

var sourceTypes: [HKVerifiableClinicalRecordSourceType]

The source for the verifiable clinical records, for example from a SMART Health Card or an EU Digital COVID Certificate.

