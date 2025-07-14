

- Address Book UI
- ABPersonViewController
-  allowsEditing Deprecated

Instance Property

# allowsEditing

Specifies whether the user can edit the person’s information.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var allowsEditing: Bool { get set }
```

Deprecated

Use CNContactViewController instead.

## Discussion

When editing a person’s information, all person properties are visible.

## See Also

### Configuring Person Views

var addressBook: ABAddressBook?

Optional. The address book from which to obtain the contact to display.

Deprecated

var allowsActions: Bool

Specifies whether the to display buttons for actions such as sending a text message or initiating a FaceTime call.

Deprecated

func setHighlightedItemForProperty(ABPropertyID, withIdentifier: ABMultiValueIdentifier)

Specifies whether to highlight a particular property of the displayed person.

Deprecated

