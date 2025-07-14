

- Contacts
- CNChangeHistoryFetchRequest
-  additionalContactKeyDescriptors 

Instance Property

# additionalContactKeyDescriptors

An array of contact property keys or key descriptors from contact objects to fetch in the returned contacts.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
var additionalContactKeyDescriptors: [any CNKeyDescriptor]? { get set }
```

## Discussion

By default, the system only fetches CNContactIdentifierKey if you do not include a list of additional key descriptors. The system always fetches CNContactIdentifierKey, whether you request it or not.

For a list of possible keys, see Contact Keys.

## See Also

### Configuring the fetch request

var excludedTransactionAuthors: [String]?

An array of strings that identify transaction authors to exclude from the fetch results.

var includeGroupChanges: Bool

A Boolean value that indicates whether the fetch should also return group changes.

var mutableObjects: Bool

A Boolean value that indicates whether the fetch should return mutable contacts and groups.

var shouldUnifyResults: Bool

A Boolean value that indicates whether the fetch should return contact changes as unified contacts.

var startingToken: Data?

An opaque token that indicates a point in history in the user’s Contacts database.

