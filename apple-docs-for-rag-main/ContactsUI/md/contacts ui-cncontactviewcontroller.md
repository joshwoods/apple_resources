

- Contacts UI
-  CNContactViewController 

Class

# CNContactViewController

A view controller that displays a new, unknown, or existing contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
@MainActor
class CNContactViewController
```

## Overview

Present a `CNContactViewController` object when you want to display information about one of the user’s contacts. At creation time, you specify the type of contact you want to display: new, unknown, or existing.

## Topics

### Creating the Contact Viewer

convenience init(for: CNContact)

Initializes a view controller for an existing contact.

convenience init(forContact: CNContact)

Initializes a view controller for an existing contact.

convenience init(forUnknownContact: CNContact)

Initializes a view controller for an unknown contact.

convenience init(forNewContact: CNContact?)

Initializes a view controller for a new contact.

### Handling Interactions with the Interface

var delegate: (any CNContactViewControllerDelegate)?

The delegate to be notified.

protocol CNContactViewControllerDelegate

Methods you use to respond to user interactions with a contact view controller.

### Required Keys

class func descriptorForRequiredKeys() -> any CNKeyDescriptor

Returns the descriptor for all the keys that must be fetched on the contact before setting it on the view controller.

### Displaying Contact Properties

var contact: CNContact

The contact being displayed.

var alternateName: String?

The name to use if the contact has no display name.

var message: String?

The message displayed under the name of the contact.

var displayedPropertyKeys: [Any]?

The contact property keys to display.

### Configuring the Contact’s Relationships

var parentGroup: CNGroup?

The group in which to add a new contact.

var parentContainer: CNContainer?

The container in which to add a new contact.

### Contact Store

var contactStore: CNContactStore?

The contact store from which the contact was fetched or to which it will be saved.

### Customizing Contact Card

var allowsEditing: Bool

Determines whether the user can edit the contact’s information.

var allowsActions: Bool

Determines whether to display buttons for actions such as sending a text message or initiating a FaceTime call.

var shouldShowLinkedContacts: Bool

Determines whether to display data from contacts that are linked to the contact being displayed.

### Highlighting a Property

func highlightProperty(withKey: String, identifier: String?)

Highlights the property of the contact being displayed.

## Relationships

### Inherits From

- NSViewController
- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
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

