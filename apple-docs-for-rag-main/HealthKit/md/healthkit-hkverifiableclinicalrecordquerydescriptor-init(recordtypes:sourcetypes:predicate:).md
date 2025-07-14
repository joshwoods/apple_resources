

- HealthKit
- HKVerifiableClinicalRecordQueryDescriptor
-  init(recordTypes:sourceTypes:predicate:) 

Initializer

# init(recordTypes:sourceTypes:predicate:)

Creates a query descriptor for reading verifiable clinical records.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOS

``` source
init(
    recordTypes: [HKVerifiableClinicalRecordCredentialType],
    sourceTypes: [HKVerifiableClinicalRecordSourceType],
    predicate: NSPredicate? = nil
)
```

## Parameters 

`recordTypes`  

The types of records that this query returns. For a list of valid record types, see HKVerifiableClinicalRecordCredentialType.

`sourceTypes`  

The format of the verifiable clinical records. For a list of valid sources, see HKVerifiableClinicalRecordSourceType.

`predicate`  

A predicate that limits the results that this query returns. Pass `nil` to receive all records of the specified source and record type.

