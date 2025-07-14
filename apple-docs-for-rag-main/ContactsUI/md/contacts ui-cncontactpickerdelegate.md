

- Contacts UI
-  CNContactPickerDelegate 

Protocol

# CNContactPickerDelegate

The methods that you implement to respond to contact-picker user events.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
protocol CNContactPickerDelegate : NSObjectProtocol
```

## Topics

### Responding to User Selections

func contactPicker(CNContactPickerViewController, didSelect: CNContact)

Called after a contact has been selected by the user.

func contactPicker(CNContactPickerViewController, didSelect: CNContactProperty)

Called when a property of the contact has been selected by the user.

func contactPicker(CNContactPickerViewController, didSelect: [CNContact])

Called after contacts have been selected by the user.

func contactPicker(CNContactPickerViewController, didSelectContactProperties: [CNContactProperty])

Called after contact properties have been selected by the user.

### Dismissing the Picker Interface

func contactPickerDidCancel(CNContactPickerViewController)

In iOS, called when the user taps Cancel.

func contactPickerWillClose(CNContactPicker)

In macOS, called when the contact picker’s popover is about to close.

func contactPickerDidClose(CNContactPicker)

In macOS, called when the contact picker’s popover has closed.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Related Documentation

var delegate: (any CNContactPickerDelegate)?

The picker delegate to be notified when the user chooses a contact.

var delegate: (any CNContactPickerDelegate)?

The delegate to be notified when the user selects a contact or a property.

### Responding to Picker Interactions

var delegate: (any CNContactPickerDelegate)?

The picker delegate to be notified when the user chooses a contact.

