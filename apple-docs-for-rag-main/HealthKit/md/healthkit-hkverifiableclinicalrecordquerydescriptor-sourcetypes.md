

- HealthKit
- HKVerifiableClinicalRecordQueryDescriptor
-  sourceTypes 

Instance Property

# sourceTypes

The source for the verifiable clinical records, for example from a SMART Health Card or an EU Digital COVID Certificate.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOS

``` source
var sourceTypes: [HKVerifiableClinicalRecordSourceType]
```

## Discussion

For a list of valid sources, see HKVerifiableClinicalRecordSourceType.

## See Also

### Accessing Query Properties

var recordTypes: [HKVerifiableClinicalRecordCredentialType]

The types of records returned by this query.

var predicate: NSPredicate?

A predicate that limits the results returned by the query.

