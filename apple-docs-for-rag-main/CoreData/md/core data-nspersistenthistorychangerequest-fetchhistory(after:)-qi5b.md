

- Core Data
- NSPersistentHistoryChangeRequest
-  fetchHistory(after:) 

Type Method

# fetchHistory(after:)

Retrieves history since a given date.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class func fetchHistory(after date: Date) -> Self
```

## Parameters 

`date`  

The date used to define the start of the fetch history.

## Return Value

A persistent history fetch request (NSPersistentHistoryChangeRequest) with an initial date boundary.

## Mentioned in 

Consuming relevant store changes

## See Also

### Fetching History

class func fetchHistory(after: NSPersistentHistoryToken?) -> Self

Retrieves the request history after a given token.

class func fetchHistory(after: NSPersistentHistoryTransaction?) -> Self

Retrieves history since a given transaction.

class func fetchHistory(withFetch: NSFetchRequest&lt;any NSFetchRequestResult>) -> Self

Retrieves history based on a fetch request.

