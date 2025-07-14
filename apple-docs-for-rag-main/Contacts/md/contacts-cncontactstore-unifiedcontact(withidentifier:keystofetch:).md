

- Contacts
- CNContactStore
-  unifiedContact(withIdentifier:keysToFetch:) 

Instance Method

# unifiedContact(withIdentifier:keysToFetch:)

Fetches a unified contact for the specified contact identifier.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
func unifiedContact(
    withIdentifier identifier: String,
    keysToFetch keys: [any CNKeyDescriptor]
) throws -> CNContact
```

## Parameters 

`identifier`  

The identifier of the contact to fetch.

`keys`  

The properties to fetch in the returned CNContact object.

## Return Value

A unified contact matching or linked to the identifier.

## Discussion

Due to unification, the returned contact may have a different identifier than you specify. To fetch a batch of contacts by identifiers, use predicateForContacts(withIdentifiers:) with unifiedContacts(matching:keysToFetch:). Fetch only the properties that your app uses. You can combine contact keys and contact key descriptors together.

To include CNContactNoteKey in the array of keys in iOS, add the com.apple.developer.contacts.notes entitlement to your app. The entitlement requires permission from Apple to use, and you can’t publicly distribute your app until you have permission to use it. For more information about adding the entitlement and getting permission, see com.apple.developer.contacts.notes.

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure. You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and About Imported Cocoa Error Parameters.

## See Also

### Fetching contacts

func enumerateContacts(with: CNContactFetchRequest, usingBlock: (CNContact, UnsafeMutablePointer&lt;ObjCBool>) -> Void) throws

Returns a Boolean value that indicates whether the enumeration of all contacts matching a contact fetch request executes successfully.

func unifiedMeContactWithKeys(toFetch: [any CNKeyDescriptor]) throws -> CNContact

Fetches the unified contact that’s the *me* card.

func unifiedContacts(matching: NSPredicate, keysToFetch: [any CNKeyDescriptor]) throws -> [CNContact]

Fetches all unified contacts matching the specified predicate.

