

- CloudKit
- CKFetchDatabaseChangesOperation
-  fetchAllChanges 

Instance Property

# fetchAllChanges

A Boolean value that indicates whether to send repeated requests to the server.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var fetchAllChanges: Bool { get set }
```

## Discussion

If true, the operation sends repeat requests to the server until it fetches all changes. CloudKit executes the handler you set on the changeTokenUpdatedBlock property with a change token after each request.

The default value is true.

## See Also

### Configuring the Operation

var previousServerChangeToken: CKServerChangeToken?

The server change token.

var resultsLimit: Int

The maximum number of results that the operation fetches.

