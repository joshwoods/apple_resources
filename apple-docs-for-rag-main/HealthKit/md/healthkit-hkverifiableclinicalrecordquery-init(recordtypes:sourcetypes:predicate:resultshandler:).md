

- HealthKit
- HKVerifiableClinicalRecordQuery
-  init(recordTypes:sourceTypes:predicate:resultsHandler:) 

Initializer

# init(recordTypes:sourceTypes:predicate:resultsHandler:)

Creates a query for one-time access to a verifiable clinical record.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOS 1.0+

``` source
init(
    recordTypes: [String],
    sourceTypes: [HKVerifiableClinicalRecordSourceType],
    predicate: NSPredicate?,
    resultsHandler: @escaping (HKVerifiableClinicalRecordQuery, [HKVerifiableClinicalRecord]?, (any Error)?) -> Void
)
```

## Parameters 

`recordTypes`  

The types of records that this query returns. For a list of valid record types, see HKVerifiableClinicalRecordCredentialType.

`sourceTypes`  

The format of the verifiable clinical records. For a list of valid sources, see HKVerifiableClinicalRecordSourceType.

`predicate`  

A predicate that limits the results that this query returns. Pass `nil` to receive all records of the specified source and record type.

`resultsHandler`  

A block that the HealthKit store calls after it finishes executing the query.

This block takes the following parameters:

`query`  
A reference to the query that called this block.

`records`  
An array containing the verifiable health records found by the query, or `nil` if an error occurs.

`error`  
If an error occurs, an object describing the error; otherwise, it’s `nil`.

## See Also

### Creating Queries

init(recordTypes: [String], predicate: NSPredicate?, resultsHandler: (HKVerifiableClinicalRecordQuery, [HKVerifiableClinicalRecord]?, (any Error)?) -> Void)

Creates a query for one-time access to a SMART Health Card.

