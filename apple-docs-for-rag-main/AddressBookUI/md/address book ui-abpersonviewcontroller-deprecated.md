

- Address Book UI
-  ABPersonViewController Deprecated

Class

# ABPersonViewController

The `ABPersonViewController` class (whose instances are known as **person view controllers**) implements the view used to display a person record (`ABPersonRef`).

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
class ABPersonViewController
```

Deprecated

Use init(for:) instead.

## Overview

Important

Person view controllers must be used with a navigation controller in order to function properly.

### Subclassing

The `ABPersonViewController` class does not support subclassing.

## Topics

### Responding to View Controller Interactions

var personViewDelegate: (any ABPersonViewControllerDelegate)?

The person-view controller delegate.

protocol ABPersonViewControllerDelegate

The `ABPersonViewControllerDelegate` protocol declares the interface that must be implemented by ABPersonViewController delegates.

### Displaying Person Properties

var displayedPerson: ABRecord

The person displayed by the person view.

var displayedProperties: [NSNumber]?

Identifies the set of properties (such as name or telephone number) of displayedPerson the receiver displays.

var shouldShowLinkedPeople: Bool

Indicates whether the person view should display data from person records that are linked with the person record being displayed.

### Configuring Person Views

var addressBook: ABAddressBook?

Optional. The address book from which to obtain the contact to display.

var allowsActions: Bool

Specifies whether the to display buttons for actions such as sending a text message or initiating a FaceTime call.

var allowsEditing: Bool

Specifies whether the user can edit the person’s information.

func setHighlightedItemForProperty(ABPropertyID, withIdentifier: ABMultiValueIdentifier)

Specifies whether to highlight a particular property of the displayed person.

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
- UIViewControllerRestoration

## See Also

### Detail Display

class ABNewPersonViewController

A view controller presenting an interface to create a contact.

Deprecated

class ABUnknownPersonViewController

The `ABUnknownPersonViewController` class (whose instances are known as **unknown-person view controllers**) implements a view controller used to create a person record from a set of person properties.

Deprecated

func ABCreateStringWithAddressDictionary([AnyHashable : Any], Bool) -> String

Returns a formatted address from an address property.

Deprecated

