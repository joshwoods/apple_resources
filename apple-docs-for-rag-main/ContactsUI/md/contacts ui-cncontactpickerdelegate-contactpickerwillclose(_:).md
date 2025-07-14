

- Contacts UI
- CNContactPickerDelegate
-  contactPickerWillClose(\_:) 

Instance Method

# contactPickerWillClose(\_:)

In macOS, called when the contact picker’s popover is about to close.

macOS 10.11+

``` source
optional func contactPickerWillClose(_ picker: CNContactPicker)
```

## Parameters 

`picker`  

The contact picker popover to be closed.

## See Also

### Dismissing the Picker Interface

func contactPickerDidCancel(CNContactPickerViewController)

In iOS, called when the user taps Cancel.

func contactPickerDidClose(CNContactPicker)

In macOS, called when the contact picker’s popover has closed.

