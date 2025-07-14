

- Contacts
- CNSaveRequest
-  shouldRefetchContacts 

Instance Property

# shouldRefetchContacts

A Boolean value that indicates whether to refetch the added and updated contacts after the save request executes.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+visionOS 1.0+

``` source
var shouldRefetchContacts: Bool { get set }
```

## Discussion

The default value is true, so the save request refetches added and updated contacts. Set to false to suppress the refetch behavior and reduce the save request’s execution time.

## See Also

### Configuring the save request

var transactionAuthor: String?

A string that identifies the author of the transaction.

