

- Core Data
- NSPersistentHistoryChangeRequest
-  fetchHistory(after:) 

Type Method

# fetchHistory(after:)

Retrieves the request history after a given token.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class func fetchHistory(after token: NSPersistentHistoryToken?) -> Self
```

## Parameters 

`token`  

The bookmark that defines the start of the request history.

## Return Value

A persistent history fetch request (NSPersistentHistoryChangeRequest) with an initial token bookmark boundary.

## Mentioned in 

Consuming relevant store changes

## See Also

### Fetching History

class func fetchHistory(after: Date) -> Self

Retrieves history since a given date.

class func fetchHistory(after: NSPersistentHistoryTransaction?) -> Self

Retrieves history since a given transaction.

class func fetchHistory(withFetch: NSFetchRequest&lt;any NSFetchRequestResult>) -> Self

Retrieves history based on a fetch request.

