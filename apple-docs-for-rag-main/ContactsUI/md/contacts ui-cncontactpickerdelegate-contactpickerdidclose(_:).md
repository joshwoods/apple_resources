

- Contacts UI
- CNContactPickerDelegate
-  contactPickerDidClose(\_:) 

Instance Method

# contactPickerDidClose(\_:)

In macOS, called when the contact picker’s popover has closed.

macOS 10.11+

``` source
optional func contactPickerDidClose(_ picker: CNContactPicker)
```

## Parameters 

`picker`  

The contact picker popover to be closed.

## See Also

### Dismissing the Picker Interface

func contactPickerDidCancel(CNContactPickerViewController)

In iOS, called when the user taps Cancel.

func contactPickerWillClose(CNContactPicker)

In macOS, called when the contact picker’s popover is about to close.

