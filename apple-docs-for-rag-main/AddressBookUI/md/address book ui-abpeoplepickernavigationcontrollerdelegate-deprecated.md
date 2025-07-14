

- Address Book UI
-  ABPeoplePickerNavigationControllerDelegate Deprecated

Protocol

# ABPeoplePickerNavigationControllerDelegate

The `ABPeoplePickerNavigationControllerDelegate` protocol describes the interface ABPeoplePickerNavigationController delegates must adopt to respond to people-picker user events.

iOS 2.0+iPadOS 2.0+Mac Catalyst 14.0+

``` source
protocol ABPeoplePickerNavigationControllerDelegate : NSObjectProtocol
```

Deprecated

Use CNContactPickerDelegate instead.

## Topics

### Responding to User Events

func peoplePickerNavigationController(ABPeoplePickerNavigationController, shouldContinueAfterSelectingPerson: ABRecord) -> Bool

Sent when the user selects a contact.

func peoplePickerNavigationController(ABPeoplePickerNavigationController, shouldContinueAfterSelectingPerson: ABRecord, property: ABPropertyID, identifier: ABMultiValueIdentifier) -> Bool

Sent when the user selects one of a person’s properties.

func peoplePickerNavigationControllerDidCancel(ABPeoplePickerNavigationController)

Sent when the user taps Cancel.

func peoplePickerNavigationController(ABPeoplePickerNavigationController, didSelectPerson: ABRecord)

Called after a person has been selected by the user.

func peoplePickerNavigationController(ABPeoplePickerNavigationController, didSelectPerson: ABRecord, property: ABPropertyID, identifier: ABMultiValueIdentifier)

Called after a property has been selected by the user.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to View Controller Interactions

var peoplePickerDelegate: (any ABPeoplePickerNavigationControllerDelegate)?

The people-picker navigation controller delegate.

Deprecated

