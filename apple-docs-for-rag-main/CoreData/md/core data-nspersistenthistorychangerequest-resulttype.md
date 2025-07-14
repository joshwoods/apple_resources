

- Core Data
- NSPersistentHistoryChangeRequest
-  resultType 

Instance Property

# resultType

The type of result that this request returns.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var resultType: NSPersistentHistoryResultType { get set }
```

## Discussion

This value defaults to NSPersistentHistoryResultType.transactionsAndChanges.

## See Also

### Configuring the Request

var fetchRequest: NSFetchRequest&lt;any NSFetchRequestResult>?

The specified fetch request, when retrieving history.

