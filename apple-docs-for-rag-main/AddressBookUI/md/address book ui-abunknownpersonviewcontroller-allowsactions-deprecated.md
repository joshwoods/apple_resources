

- Address Book UI
- ABUnknownPersonViewController
-  allowsActions Deprecated

Instance Property

# allowsActions

Specifies whether buttons appear to let the user perform actions such as sharing the contact, initiating a FaceTime call, or sending a text message.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var allowsActions: Bool { get set }
```

Deprecated

Use CNContactViewController instead.

## Discussion

The default value is false.

## See Also

### Configuring the Interface Details

var addressBook: ABAddressBook?

Optional. The address book database that the person record is added to.

Deprecated

var allowsAddingToAddressBook: Bool

Specifies whether the user can add the properties displayed by the unknown-person view controller to the address book database, either as a new contact or by adding them to an existing contact.

Deprecated

