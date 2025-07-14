

- Core Data
- NSAsynchronousFetchRequest
-  estimatedResultCount 

Instance Property

# estimatedResultCount

A configuration parameter that assists Core Data with scheduling the asynchronous fetch request.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var estimatedResultCount: Int { get set }
```

## See Also

### Preparing a Request

var completionBlock: NSPersistentStoreAsynchronousFetchResultCompletionBlock?

The block that is executed when the fetch request has completed.

var fetchRequest: NSFetchRequest&lt;ResultType>

The underlying fetch request that is executed asynchronously.

