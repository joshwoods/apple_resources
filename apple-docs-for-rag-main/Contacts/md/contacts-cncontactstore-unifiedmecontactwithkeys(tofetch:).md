

- Contacts
- CNContactStore
-  unifiedMeContactWithKeys(toFetch:) 

Instance Method

# unifiedMeContactWithKeys(toFetch:)

Fetches the unified contact that’s the *me* card.

macOS 10.11+

``` source
func unifiedMeContactWithKeys(toFetch keys: [any CNKeyDescriptor]) throws -> CNContact
```

## Parameters 

`keys`  

The properties to fetch in the returned CNContact object.

## Return Value

The unified contact that is the *me* card or `nil` if there isn’t one.

## Discussion

In the user interface, *My Card* represents the *me* contact. Fetch only the properties your app uses. You can combine contact keys and contact key descriptors together.

To include CNContactNoteKey in the array of keys in iOS 13 or later or macOS 13 or later, add the com.apple.developer.contacts.notes entitlement to your app. The entitlement requires permission from Apple to use, and you can’t publicly distribute your app until you have permission to use it. For more information about adding the entitlement and getting permission, see com.apple.developer.contacts.notes.

## See Also

### Fetching contacts

func enumerateContacts(with: CNContactFetchRequest, usingBlock: (CNContact, UnsafeMutablePointer&lt;ObjCBool>) -> Void) throws

Returns a Boolean value that indicates whether the enumeration of all contacts matching a contact fetch request executes successfully.

func unifiedContact(withIdentifier: String, keysToFetch: [any CNKeyDescriptor]) throws -> CNContact

Fetches a unified contact for the specified contact identifier.

func unifiedContacts(matching: NSPredicate, keysToFetch: [any CNKeyDescriptor]) throws -> [CNContact]

Fetches all unified contacts matching the specified predicate.

