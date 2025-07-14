

- Contacts
- CNFetchResult
-  currentHistoryToken 

Instance Property

# currentHistoryToken

An opaque token that indicates a point in history in the user’s Contacts database.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
var currentHistoryToken: Data { get }
```

## Discussion

Save this token after a successful change history fetch result in your app. Then, set the saved token in startingToken in a subsequent CNChangeHistoryFetchRequest to receive changes after that point in history.

## See Also

### Accessing results

var value: ValueType

The result of the fetch request, expressed as the value type you specify.

