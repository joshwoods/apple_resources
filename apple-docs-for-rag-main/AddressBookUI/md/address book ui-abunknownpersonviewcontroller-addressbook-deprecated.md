

- Address Book UI
- ABUnknownPersonViewController
-  addressBook Deprecated

Instance Property

# addressBook

Optional. The address book database that the person record is added to.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var addressBook: ABAddressBook? { get set }
```

Deprecated

Use CNContactViewController instead.

## Discussion

When unspecified, this view controller sets the value of this property by creating an `ABAddressBookRef` object.

The person record is only added to the address book database if allowsAddingToAddressBook is true and the user taps the “Add to Existing Contact” or “Create New Contact” button.

## See Also

### Configuring the Interface Details

var allowsActions: Bool

Specifies whether buttons appear to let the user perform actions such as sharing the contact, initiating a FaceTime call, or sending a text message.

Deprecated

var allowsAddingToAddressBook: Bool

Specifies whether the user can add the properties displayed by the unknown-person view controller to the address book database, either as a new contact or by adding them to an existing contact.

Deprecated

