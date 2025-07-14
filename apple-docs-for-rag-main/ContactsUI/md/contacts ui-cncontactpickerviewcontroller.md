

- Contacts UI
-  CNContactPickerViewController 

Class

# CNContactPickerViewController

A view controller that displays an interface for picking contacts.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class CNContactPickerViewController
```

## Overview

A CNContactPickerViewController allows the user to select one or more contacts (or their properties) from the list of contacts displayed in the contact view controller (CNContactViewController). The picker supports both single selection and multiselection of the contacts. The app using contact picker view does not need access to the user’s contacts and the user will not be prompted for “grant permission” access. The app has access only to the user’s final selection.

There are predefined predicates in this class that let you control the user selection of the contact. Changing the predicates only take effect before the view is presented.

## Topics

### Displaying Contacts Properties

var displayedPropertyKeys: [String]?

The CNContact property keys to display in the contact detail card.

### Responding to User Interactions

var delegate: (any CNContactPickerDelegate)?

The delegate to be notified when the user selects a contact or a property.

protocol CNContactPickerDelegate

The methods that you implement to respond to contact-picker user events.

### Predicates For Selecting Contacts

var predicateForEnablingContact: NSPredicate?

A predicate to determine the contact selectability in the list of contacts.

var predicateForSelectionOfContact: NSPredicate?

A predicate to control the return of the selected contact.

var predicateForSelectionOfProperty: NSPredicate?

A predicate to control the properties of the selected contact.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Contact pickers

class CNContactPicker

A popover-based interface for selecting a contact.

