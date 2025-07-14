

- Address Book UI
- ABPersonViewController
-  allowsActions Deprecated

Instance Property

# allowsActions

Specifies whether the to display buttons for actions such as sending a text message or initiating a FaceTime call.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var allowsActions: Bool { get set }
```

Deprecated

Use CNContactViewController instead.

## See Also

### Configuring Person Views

var addressBook: ABAddressBook?

Optional. The address book from which to obtain the contact to display.

Deprecated

var allowsEditing: Bool

Specifies whether the user can edit the person’s information.

Deprecated

func setHighlightedItemForProperty(ABPropertyID, withIdentifier: ABMultiValueIdentifier)

Specifies whether to highlight a particular property of the displayed person.

Deprecated

