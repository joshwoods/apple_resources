

- Core Data
- NSPersistentHistoryChangeRequest
-  deleteHistory(before:) 

Type Method

# deleteHistory(before:)

Purges history older than a given date.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class func deleteHistory(before date: Date) -> Self
```

## Parameters 

`date`  

The date used to define the end of the delete history request.

## Return Value

A delete history change request (NSPersistentHistoryChangeRequest) using an end date boundary.

## See Also

### Purging History

class func deleteHistory(before: NSPersistentHistoryToken?) -> Self

Purges history older than that defined by a given token.

class func deleteHistory(before: NSPersistentHistoryTransaction?) -> Self

Purges history older than a given transaction.

