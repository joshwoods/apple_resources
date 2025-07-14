

- Contacts
- CNContactStore
-  enumerateContacts(with:usingBlock:) 

Instance Method

# enumerateContacts(with:usingBlock:)

Returns a Boolean value that indicates whether the enumeration of all contacts matching a contact fetch request executes successfully.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
func enumerateContacts(
    with fetchRequest: CNContactFetchRequest,
    usingBlock block: (CNContact, UnsafeMutablePointer) -> Void
) throws
```

## Parameters 

`fetchRequest`  

The contact fetch request that specifies the search criteria.

`block`  

Called for each contact matching the fetch request.

## Return Value

true if enumeration of all contacts matching a contact fetch request executes successfully; otherwise, false.

## Discussion

This method waits until the enumeration is finished. If there are no results, the block is not called and the method returns true.

This method can fetch all contacts without keeping all of them at once in memory, which is expensive.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure. You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and About Imported Cocoa Error Parameters.

## See Also

### Fetching contacts

func unifiedMeContactWithKeys(toFetch: [any CNKeyDescriptor]) throws -> CNContact

Fetches the unified contact that’s the *me* card.

func unifiedContact(withIdentifier: String, keysToFetch: [any CNKeyDescriptor]) throws -> CNContact

Fetches a unified contact for the specified contact identifier.

func unifiedContacts(matching: NSPredicate, keysToFetch: [any CNKeyDescriptor]) throws -> [CNContact]

Fetches all unified contacts matching the specified predicate.

