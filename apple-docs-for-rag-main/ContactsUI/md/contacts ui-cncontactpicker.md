

- Contacts UI
-  CNContactPicker 

Class

# CNContactPicker

A popover-based interface for selecting a contact.

macOS 10.11+

``` source
class CNContactPicker
```

## Overview

Before displaying the popover, configure the displayedKeys property with the information you want to display in the interface.

## Topics

### Responding to Picker Interactions

var delegate: (any CNContactPickerDelegate)?

The picker delegate to be notified when the user chooses a contact.

protocol CNContactPickerDelegate

The methods that you implement to respond to contact-picker user events.

### Configuring the Picker Contents

var displayedKeys: [String]

The keys to be displayed when a contact is expanded.

### Displaying the Popover

func showRelative(to: NSRect, of: NSView, preferredEdge: NSRectEdge)

Shows the picker popover anchored to the specified view.

### Closing the Popover

func close()

Closes the popover.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Contact pickers

class CNContactPickerViewController

A view controller that displays an interface for picking contacts.

