

- Contacts UI
- CNContactPickerDelegate
-  contactPickerDidCancel(\_:) 

Instance Method

# contactPickerDidCancel(\_:)

In iOS, called when the user taps Cancel.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func contactPickerDidCancel(_ picker: CNContactPickerViewController)
```

## Parameters 

`picker`  

The contact picker in which the selection was made.

## Discussion

The picker is dismissed automatically after a contact or property is picked.

## See Also

### Dismissing the Picker Interface

func contactPickerWillClose(CNContactPicker)

In macOS, called when the contact picker’s popover is about to close.

func contactPickerDidClose(CNContactPicker)

In macOS, called when the contact picker’s popover has closed.

