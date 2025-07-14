

- HealthKit
- HKVerifiableClinicalRecordQuery
-  init(recordTypes:predicate:resultsHandler:) 

Initializer

# init(recordTypes:predicate:resultsHandler:)

Creates a query for one-time access to a SMART Health Card.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
init(
    recordTypes: [String],
    predicate: NSPredicate?,
    resultsHandler: @escaping (HKVerifiableClinicalRecordQuery, [HKVerifiableClinicalRecord]?, (any Error)?) -> Void
)
```

## Parameters 

`recordTypes`  

The types of records that the query returns.

`predicate`  

A predicate that limits the results that they query returns. Pass `nil` to receive all records of the specified type.

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

init(recordTypes: [String], sourceTypes: [HKVerifiableClinicalRecordSourceType], predicate: NSPredicate?, resultsHandler: (HKVerifiableClinicalRecordQuery, [HKVerifiableClinicalRecord]?, (any Error)?) -> Void)

Creates a query for one-time access to a verifiable clinical record.

