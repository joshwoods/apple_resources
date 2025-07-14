

- Contacts UI
- CNContactPicker
-  delegate 

Instance Property

# delegate

The picker delegate to be notified when the user chooses a contact.

macOS 10.11+

``` source
weak var delegate: (any CNContactPickerDelegate)? { get set }
```

## See Also

### Responding to Picker Interactions

protocol CNContactPickerDelegate

The methods that you implement to respond to contact-picker user events.

