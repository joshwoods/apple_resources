

- CloudKit
- CKFetchShareMetadataOperation
-  shareURLs 

Instance Property

# shareURLs

The URLs of the shares to fetch.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var shareURLs: [URL]? { get set }
```

## Discussion

Use this property to view or change the URLs of the shares to fetch. If you intend to specify or change this property’s value, do so before you execute the operation or submit it to a queue.

## See Also

### Configuring the Operation

var shouldFetchRootRecord: Bool

A Boolean value that indicates whether to retrieve the root record.

