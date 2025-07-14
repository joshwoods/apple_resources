

- Address Book UI
-  ABNewPersonViewController Deprecated

Class

# ABNewPersonViewController

A view controller presenting an interface to create a contact.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
class ABNewPersonViewController
```

Deprecated

Use CNContactViewController instead.

## Overview

New-person view controllers are modal view controllers that manage a set of view controllers used to create a contact (`ABPersonRef`) and edit its properties.

Important

New-person view controllers must be used with a navigation controller in order to function properly. It is recommended that you present a new-person view controller modally.

### Subclassing

The `ABNewPersonViewController` class does not support subclassing.

## Topics

### Responding to View Controller Interactions

var newPersonViewDelegate: (any ABNewPersonViewControllerDelegate)?

The delegate of a new-person view controller.

protocol ABNewPersonViewControllerDelegate

The `ABNewPersonViewControllerDelegate` protocol declares the interface that ABNewPersonViewController delegates must implement.

### Displaying Person Properties

var displayedPerson: ABRecord?

Optional. Specifies the person properties that the new-person view controller pre-fills in its views.

### Configuring New Person Views

var addressBook: ABAddressBook?

Optional. The address book to which the new contact is added.

var parentGroup: ABRecord?

Optional. Specifies the group to which to add the new contact on save.

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

### Detail Display

class ABPersonViewController

The `ABPersonViewController` class (whose instances are known as **person view controllers**) implements the view used to display a person record (`ABPersonRef`).

Deprecated

class ABUnknownPersonViewController

The `ABUnknownPersonViewController` class (whose instances are known as **unknown-person view controllers**) implements a view controller used to create a person record from a set of person properties.

Deprecated

func ABCreateStringWithAddressDictionary([AnyHashable : Any], Bool) -> String

Returns a formatted address from an address property.

Deprecated

