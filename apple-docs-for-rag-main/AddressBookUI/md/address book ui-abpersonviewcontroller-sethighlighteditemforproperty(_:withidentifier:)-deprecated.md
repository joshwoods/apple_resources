

- Address Book UI
- ABPersonViewController
-  setHighlightedItemForProperty(\_:withIdentifier:) Deprecated

Instance Method

# setHighlightedItemForProperty(\_:withIdentifier:)

Specifies whether to highlight a particular property of the displayed person.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func setHighlightedItemForProperty(
    _ property: ABPropertyID,
    withIdentifier identifier: ABMultiValueIdentifier
)
```

Deprecated

Use CNContactViewController instead.

## Parameters 

`property`  

The property to highlight.

`identifier`  

When `property` is a multi-value property, the value to highlight.

## See Also

### Configuring Person Views

var addressBook: ABAddressBook?

Optional. The address book from which to obtain the contact to display.

Deprecated

var allowsActions: Bool

Specifies whether the to display buttons for actions such as sending a text message or initiating a FaceTime call.

Deprecated

var allowsEditing: Bool

Specifies whether the user can edit the person’s information.

Deprecated

