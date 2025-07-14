

- CloudKit
- CKFetchShareMetadataOperation
-  shouldFetchRootRecord 

Instance Property

# shouldFetchRootRecord

A Boolean value that indicates whether to retrieve the root record.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var shouldFetchRootRecord: Bool { get set }
```

## Discussion

For a shared record hierarchy, set this property to true to include the root record in the fetched share metadata. CloudKit ignores this property for a shared record zone because, unlike a shared record hierarchy, it doesn’t have a nominated root record.

The default value is false.

## See Also

### Configuring the Operation

var shareURLs: [URL]?

The URLs of the shares to fetch.

