

- Contacts UI
- CNContactPickerDelegate
-  contactPicker(\_:didSelect:) 

Instance Method

# contactPicker(\_:didSelect:)

Called after contacts have been selected by the user.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func contactPicker(
    _ picker: CNContactPickerViewController,
    didSelect contacts: [CNContact]
)
```

## Parameters 

`picker`  

The contact picker where the selection was made.

`contacts`  

The selected contacts.

## Discussion

This delegate method is called when the user selects more than one contact. Implementing this method configures the picker for multi-selection.

## See Also

### Responding to User Selections

func contactPicker(CNContactPickerViewController, didSelect: CNContact)

Called after a contact has been selected by the user.

func contactPicker(CNContactPickerViewController, didSelect: CNContactProperty)

Called when a property of the contact has been selected by the user.

func contactPicker(CNContactPickerViewController, didSelectContactProperties: [CNContactProperty])

Called after contact properties have been selected by the user.

