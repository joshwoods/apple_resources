

- CloudKit
- CKQuery
-  predicate 

Instance Property

# predicate

The predicate to use for matching records.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var predicate: NSPredicate { get }
```

## Discussion

A predicate contains one or more expressions that evaluate to true or false. Expressions are often value-based comparisons, but predicates support other types of operators, including string comparisons and aggregate operations. For guidelines on how to construct predicates for your queries, see Predicate Rules for Query Objects.

## See Also

### Accessing the Query Parameters

var recordType: CKRecord.RecordType

The record type to search.

var sortDescriptors: [NSSortDescriptor]?

The sort descriptors for organizing the query’s results.

