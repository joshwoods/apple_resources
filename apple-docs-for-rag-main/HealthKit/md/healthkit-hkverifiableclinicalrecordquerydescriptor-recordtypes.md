

- HealthKit
- HKVerifiableClinicalRecordQueryDescriptor
-  recordTypes 

Instance Property

# recordTypes

The types of records returned by this query.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOS

``` source
var recordTypes: [HKVerifiableClinicalRecordCredentialType]
```

## Discussion

For a list of valid record types, see HKVerifiableClinicalRecordCredentialType.

## See Also

### Accessing Query Properties

var sourceTypes: [HKVerifiableClinicalRecordSourceType]

The source for the verifiable clinical records, for example from a SMART Health Card or an EU Digital COVID Certificate.

var predicate: NSPredicate?

A predicate that limits the results returned by the query.

