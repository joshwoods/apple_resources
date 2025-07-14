

- Core Data
- NSAsynchronousFetchRequest
-  completionBlock 

Instance Property

# completionBlock

The block that is executed when the fetch request has completed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var completionBlock: NSPersistentStoreAsynchronousFetchResultCompletionBlock? { get }
```

## See Also

### Preparing a Request

var estimatedResultCount: Int

A configuration parameter that assists Core Data with scheduling the asynchronous fetch request.

var fetchRequest: NSFetchRequest&lt;ResultType>

The underlying fetch request that is executed asynchronously.

