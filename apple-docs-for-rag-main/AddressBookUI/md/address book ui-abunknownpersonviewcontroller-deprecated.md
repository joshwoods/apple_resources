

- Address Book UI
-  ABUnknownPersonViewController Deprecated

Class

# ABUnknownPersonViewController

The `ABUnknownPersonViewController` class (whose instances are known as **unknown-person view controllers**) implements a view controller used to create a person record from a set of person properties.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
class ABUnknownPersonViewController
```

Deprecated

Use init(forUnknownContact:) instead.

## Overview

Unknown-person view controllers display contact information that can be saved to the Address Book database. From instances of this class, users may also initiate standard actions, such as:

- Phone call

- Text message

- Create contact

- Add to contact

Performing any of the standard actions may result in your application being moved to the background.

Important

Unknown-person view controllers must be used with a navigation controller in order to function properly.

### Subclassing

The `ABUnknownPersonViewController` class does not support subclassing.

## Topics

### Responding to View Controller Interactions

var unknownPersonViewDelegate: (any ABUnknownPersonViewControllerDelegate)?

The unknown-person view controller delegate.

protocol ABUnknownPersonViewControllerDelegate

The methods you use to respond to events in an unknown person view controller.

### Displaying Person Properties

var alternateName: String?

Provides a value that is displayed instead of the first and last name.

var message: String?

Text displayed below alternateName.

var displayedPerson: ABRecord

Specifies a person record whose properties are displayed by the view controller.

### Configuring the Interface Details

var addressBook: ABAddressBook?

Optional. The address book database that the person record is added to.

var allowsActions: Bool

Specifies whether buttons appear to let the user perform actions such as sharing the contact, initiating a FaceTime call, or sending a text message.

var allowsAddingToAddressBook: Bool

Specifies whether the user can add the properties displayed by the unknown-person view controller to the address book database, either as a new contact or by adding them to an existing contact.

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

## See Also

### Detail Display

class ABNewPersonViewController

A view controller presenting an interface to create a contact.

Deprecated

class ABPersonViewController

The `ABPersonViewController` class (whose instances are known as **person view controllers**) implements the view used to display a person record (`ABPersonRef`).

Deprecated

func ABCreateStringWithAddressDictionary([AnyHashable : Any], Bool) -> String

Returns a formatted address from an address property.

Deprecated

