

- Core Data
-  NSPersistentHistoryChangeRequest 

Class

# NSPersistentHistoryChangeRequest

A request to fetch or purge persistent history.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class NSPersistentHistoryChangeRequest
```

## Mentioned in 

Consuming relevant store changes

## Topics

### Configuring the Request

var fetchRequest: NSFetchRequest&lt;any NSFetchRequestResult>?

The specified fetch request, when retrieving history.

var resultType: NSPersistentHistoryResultType

The type of result that this request returns.

### Getting the Token

var token: NSPersistentHistoryToken?

The specified token, when retrieving history defined by a token.

### Fetching History

class func fetchHistory(after: Date) -> Self

Retrieves history since a given date.

class func fetchHistory(after: NSPersistentHistoryToken?) -> Self

Retrieves the request history after a given token.

class func fetchHistory(after: NSPersistentHistoryTransaction?) -> Self

Retrieves history since a given transaction.

class func fetchHistory(withFetch: NSFetchRequest&lt;any NSFetchRequestResult>) -> Self

Retrieves history based on a fetch request.

### Purging History

class func deleteHistory(before: Date) -> Self

Purges history older than a given date.

class func deleteHistory(before: NSPersistentHistoryToken?) -> Self

Purges history older than that defined by a given token.

class func deleteHistory(before: NSPersistentHistoryTransaction?) -> Self

Purges history older than a given transaction.

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

### Requesting History

class NSPersistentHistoryResult

The result of a request to fetch persistent history.

