

- Contacts UI
- CNContactPickerDelegate
-  contactPicker(\_:didSelect:) 

Instance Method

# contactPicker(\_:didSelect:)

Called after a contact has been selected by the user.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

**macOS**

``` source
optional func contactPicker(
    _ picker: CNContactPicker,
    didSelect contact: CNContact
)
```

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
optional func contactPicker(
    _ picker: CNContactPickerViewController,
    didSelect contact: CNContact
)
```

## Parameters 

`picker`  

The contact picker where the selection was made.

`contact`  

The selected contact.

## Discussion

This delegate method is called when the user selects a single contact.

## See Also

### Responding to User Selections

func contactPicker(CNContactPickerViewController, didSelect: CNContactProperty)

Called when a property of the contact has been selected by the user.

func contactPicker(CNContactPickerViewController, didSelect: [CNContact])

Called after contacts have been selected by the user.

func contactPicker(CNContactPickerViewController, didSelectContactProperties: [CNContactProperty])

Called after contact properties have been selected by the user.

