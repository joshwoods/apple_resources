

- Contacts UI
- CNContactPickerDelegate
-  contactPicker(\_:didSelect:) 

Instance Method

# contactPicker(\_:didSelect:)

Called when a property of the contact has been selected by the user.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
optional func contactPicker(
    _ picker: CNContactPickerViewController,
    didSelect contactProperty: CNContactProperty
)
```

**macOS**

``` source
optional func contactPicker(
    _ picker: CNContactPicker,
    didSelect contactProperty: CNContactProperty
)
```

## Parameters 

`picker`  

The contact picker where the selection was made.

`contactProperty`  

The selected contact property.

## Discussion

This delegate method ia called when the user selects a single property of the contact.

## See Also

### Responding to User Selections

func contactPicker(CNContactPickerViewController, didSelect: CNContact)

Called after a contact has been selected by the user.

func contactPicker(CNContactPickerViewController, didSelect: [CNContact])

Called after contacts have been selected by the user.

func contactPicker(CNContactPickerViewController, didSelectContactProperties: [CNContactProperty])

Called after contact properties have been selected by the user.

