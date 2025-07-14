

- Core Data
-  NSAsynchronousFetchRequest 

Class

# NSAsynchronousFetchRequest

A fetch request that retrieves results asynchronously and supports progress notification.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class NSAsynchronousFetchRequest where ResultType : NSFetchRequestResult
```

## Topics

### Initializing a Request

init(fetchRequest: NSFetchRequest&lt;ResultType>, completionBlock: ((NSAsynchronousFetchResult&lt;ResultType>) -> Void)?)

Initializes a new asynchronous fetch request configured with the provided fetch request and completion block.

### Preparing a Request

var completionBlock: NSPersistentStoreAsynchronousFetchResultCompletionBlock?

The block that is executed when the fetch request has completed.

var estimatedResultCount: Int

A configuration parameter that assists Core Data with scheduling the asynchronous fetch request.

var fetchRequest: NSFetchRequest&lt;ResultType>

The underlying fetch request that is executed asynchronously.

## Relationships

### Inherits From

- NSPersistentStoreRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Fetch requests

class NSFetchRequest

A description of search criteria used to retrieve data from a persistent store.

class NSAsynchronousFetchResult

A fetch result object that encompasses the response from an executed asynchronous fetch request.

class NSFetchedResultsController

A controller that you use to manage the results of a Core Data fetch request and to display data to the user.

