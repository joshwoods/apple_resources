

- Address Book UI
- ABPersonViewController
-  addressBook Deprecated

Instance Property

# addressBook

Optional. The address book from which to obtain the contact to display.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var addressBook: ABAddressBook? { get set }
```

Deprecated

Use CNContactViewController instead.

## Discussion

When unset, an address book is created and assigned to this property when needed.

## See Also

### Configuring Person Views

var allowsActions: Bool

Specifies whether the to display buttons for actions such as sending a text message or initiating a FaceTime call.

Deprecated

var allowsEditing: Bool

Specifies whether the user can edit the person’s information.

Deprecated

func setHighlightedItemForProperty(ABPropertyID, withIdentifier: ABMultiValueIdentifier)

Specifies whether to highlight a particular property of the displayed person.

Deprecated

