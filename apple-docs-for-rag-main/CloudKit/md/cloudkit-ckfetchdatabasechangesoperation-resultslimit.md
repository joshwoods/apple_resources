

- CloudKit
- CKFetchDatabaseChangesOperation
-  resultsLimit 

Instance Property

# resultsLimit

The maximum number of results that the operation fetches.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var resultsLimit: Int { get set }
```

## Discussion

Use this property to limit the number of changes this operation returns. When the operation reaches the limit, it updates the change token and returns it to indicate that more results are available.

## See Also

### Configuring the Operation

var fetchAllChanges: Bool

A Boolean value that indicates whether to send repeated requests to the server.

var previousServerChangeToken: CKServerChangeToken?

The server change token.

