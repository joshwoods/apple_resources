

- HealthKit
- HKDocumentQuery
-  sortDescriptors 

Instance Property

# sortDescriptors

An array of sort descriptors that specify the order of the results returned by this query.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 3.0+

``` source
var sortDescriptors: [NSSortDescriptor]? { get }
```

## Discussion

This property contains the value passed to the init(documentType:predicate:limit:sortDescriptors:includeDocumentData:resultsHandler:) method’s `sortDescriptors` parameter.

## See Also

### Accessing the Document Query’s Properties

var includeDocumentData: Bool

A Boolean value that indicates whether the sample includes the full document’s data.

var limit: Int

The maximum number of documents the receiver will return upon completion.

