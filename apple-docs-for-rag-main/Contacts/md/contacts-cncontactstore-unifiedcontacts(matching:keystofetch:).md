

- Contacts
- CNContactStore
-  unifiedContacts(matching:keysToFetch:) 

Instance Method

# unifiedContacts(matching:keysToFetch:)

Fetches all unified contacts matching the specified predicate.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
func unifiedContacts(
    matching predicate: NSPredicate,
    keysToFetch keys: [any CNKeyDescriptor]
) throws -> [CNContact]
```

## Parameters 

`predicate`  

The predicate to match against.

`keys`  

The properties to fetch in the returned CNContact objects. Fetch only the properties that your app uses. You can combine contact keys and contact key descriptors.

## Return Value

An array of CNContact objects matching the predicate.

## Discussion

If the system doesn’t find any matches, this method returns an empty array (or `nil` in case of error). Use only the predicates from the CNContact class predicates. This method doesn’t support compound predicates. Due to unification, the returned contacts may have different identifiers than you specify. To fetch all contacts, use enumerateContacts(with:usingBlock:).

To include CNContactNoteKey in the array of keys in iOS, add the com.apple.developer.contacts.notes entitlement to your app. The entitlement requires permission from Apple to use, and you can’t publicly distribute your app until you have permission to use it. For more information about adding the entitlement and getting permission, see com.apple.developer.contacts.notes.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure. You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and About Imported Cocoa Error Parameters.

## See Also

### Fetching contacts

func enumerateContacts(with: CNContactFetchRequest, usingBlock: (CNContact, UnsafeMutablePointer&lt;ObjCBool>) -> Void) throws

Returns a Boolean value that indicates whether the enumeration of all contacts matching a contact fetch request executes successfully.

func unifiedMeContactWithKeys(toFetch: [any CNKeyDescriptor]) throws -> CNContact

Fetches the unified contact that’s the *me* card.

func unifiedContact(withIdentifier: String, keysToFetch: [any CNKeyDescriptor]) throws -> CNContact

Fetches a unified contact for the specified contact identifier.

