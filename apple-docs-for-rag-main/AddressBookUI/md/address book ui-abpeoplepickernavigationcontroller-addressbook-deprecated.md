

- Address Book UI
- ABPeoplePickerNavigationController
-  addressBook Deprecated

Instance Property

# addressBook

Optional; the address book from which to obtain the list of contacts.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var addressBook: ABAddressBook? { get set }
```

Deprecated

Use CNContactPickerViewController instead.

## Discussion

When unset, an address book is created and assigned to this property when needed. This property is only used when the app has access to the user’s contacts—otherwise it remains `NULL`.

