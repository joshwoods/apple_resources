

- Address Book UI
-  ABPeoplePickerNavigationController Deprecated

Class

# ABPeoplePickerNavigationController

The `ABPeoplePickerNavigationController` class (whose instances are known as **people-picker navigation controllers**) implements a view controller that manages a set of views that allow the user to select a contact or one of its contact-information items from an address book.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
class ABPeoplePickerNavigationController
```

Deprecated

Use CNContactPickerViewController instead.

## Overview

In iOS 8 and later bringing up a people-picker navigtion controller does not require the app to have access to a user’s contacts, and the user will not be prompted to grant access. If the app does not itself have access to the user’s contacts, a temporary copy of the contact selected by the user will be returned to the app.

See PeoplePicker: Picking a Person or Property for a sample project illustrating the use of a people-picker navigation controller.

### Subclassing

The `ABPeoplePickerNavigationController` class does not support subclassing.

## Topics

### Responding to View Controller Interactions

var peoplePickerDelegate: (any ABPeoplePickerNavigationControllerDelegate)?

The people-picker navigation controller delegate.

protocol ABPeoplePickerNavigationControllerDelegate

The `ABPeoplePickerNavigationControllerDelegate` protocol describes the interface ABPeoplePickerNavigationController delegates must adopt to respond to people-picker user events.

### Displaying Person Properties

var displayedProperties: [NSNumber]?

The properties (such as name or telephone number) the picker displays when it shows a person.

### Configuring People Pickers

var addressBook: ABAddressBook?

Optional; the address book from which to obtain the list of contacts.

### Customizing Display and Selection

var predicateForEnablingPerson: NSPredicate?

Optionally determines if a person can be selected.

var predicateForSelectionOfPerson: NSPredicate?

Optionally determines if a selected person should be returned to the app or displayed.

var predicateForSelectionOfProperty: NSPredicate?

Optionally determines if a selected property should be returned to the app or if the default action for the property should be performed

### Constants

Address Book Properties

These constants can be used in predicates for selecting people or properties. A labeled value is an object with a “label” property and a “value” property.

## Relationships

### Inherits From

- UINavigationController

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
- Sendable
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

