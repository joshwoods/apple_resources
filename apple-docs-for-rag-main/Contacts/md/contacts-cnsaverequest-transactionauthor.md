

- Contacts
- CNSaveRequest
-  transactionAuthor 

Instance Property

# transactionAuthor

A string that identifies the author of the transaction.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
var transactionAuthor: String? { get set }
```

## Discussion

Specify a string to identify a transaction author when you save changes. Then, when you configure a CNChangeHistoryFetchRequest, provide the same string in excludedTransactionAuthors to prevent fetching changes that the author already knows about.

## See Also

### Configuring the save request

var shouldRefetchContacts: Bool

A Boolean value that indicates whether to refetch the added and updated contacts after the save request executes.

