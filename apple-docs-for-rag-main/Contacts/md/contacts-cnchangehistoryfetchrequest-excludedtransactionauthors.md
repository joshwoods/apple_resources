

- Contacts
- CNChangeHistoryFetchRequest
-  excludedTransactionAuthors 

Instance Property

# excludedTransactionAuthors

An array of strings that identify transaction authors to exclude from the fetch results.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
var excludedTransactionAuthors: [String]? { get set }
```

## Discussion

Specify authors using the same string(s) that you use in CNSaveRequest’s transactionAuthor to suppress processing changes that you already know about.

## See Also

### Configuring the fetch request

var additionalContactKeyDescriptors: [any CNKeyDescriptor]?

An array of contact property keys or key descriptors from contact objects to fetch in the returned contacts.

var includeGroupChanges: Bool

A Boolean value that indicates whether the fetch should also return group changes.

var mutableObjects: Bool

A Boolean value that indicates whether the fetch should return mutable contacts and groups.

var shouldUnifyResults: Bool

A Boolean value that indicates whether the fetch should return contact changes as unified contacts.

var startingToken: Data?

An opaque token that indicates a point in history in the user’s Contacts database.

