

- Core Data
- NSPersistentHistoryChangeRequest
-  fetchHistory(withFetch:) 

Type Method

# fetchHistory(withFetch:)

Retrieves history based on a fetch request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class func fetchHistory(withFetch fetchRequest: NSFetchRequest) -> Self
```

## Parameters 

`fetchRequest`  

The fetch request that defines the history bounds.

## Return Value

A persistent history fetch request (NSPersistentHistoryChangeRequest) built using an existing fetch request.

## See Also

### Fetching History

class func fetchHistory(after: Date) -> Self

Retrieves history since a given date.

class func fetchHistory(after: NSPersistentHistoryToken?) -> Self

Retrieves the request history after a given token.

class func fetchHistory(after: NSPersistentHistoryTransaction?) -> Self

Retrieves history since a given transaction.

