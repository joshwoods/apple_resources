

- Contacts
- CNChangeHistoryFetchRequest
-  startingToken 

Instance Property

# startingToken

An opaque token that indicates a point in history in the user’s Contacts database.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
var startingToken: Data? { get set }
```

## Discussion

Specify nil to receive a CNChangeHistoryDropEverythingEvent, followed by an add event for every contact and group in the Contacts database.

Save the currentHistoryToken from a successful fetch result in your app, then specify it here to receive changes after that point in history.

## See Also

### Configuring the fetch request

var additionalContactKeyDescriptors: [any CNKeyDescriptor]?

An array of contact property keys or key descriptors from contact objects to fetch in the returned contacts.

var excludedTransactionAuthors: [String]?

An array of strings that identify transaction authors to exclude from the fetch results.

var includeGroupChanges: Bool

A Boolean value that indicates whether the fetch should also return group changes.

var mutableObjects: Bool

A Boolean value that indicates whether the fetch should return mutable contacts and groups.

var shouldUnifyResults: Bool

A Boolean value that indicates whether the fetch should return contact changes as unified contacts.

