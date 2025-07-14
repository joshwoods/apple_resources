

- Core Data
- NSAsynchronousFetchRequest
-  fetchRequest 

Instance Property

# fetchRequest

The underlying fetch request that is executed asynchronously.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var fetchRequest: NSFetchRequest { get }
```

## See Also

### Preparing a Request

var completionBlock: NSPersistentStoreAsynchronousFetchResultCompletionBlock?

The block that is executed when the fetch request has completed.

var estimatedResultCount: Int

A configuration parameter that assists Core Data with scheduling the asynchronous fetch request.

