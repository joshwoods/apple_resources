

- Address Book UI
- ABPeoplePickerNavigationControllerDelegate
-  peoplePickerNavigationController(\_:shouldContinueAfterSelectingPerson:) Deprecated

Instance Method

# peoplePickerNavigationController(\_:shouldContinueAfterSelectingPerson:)

Sent when the user selects a contact.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
optional func peoplePickerNavigationController(
    _ peoplePicker: ABPeoplePickerNavigationController,
    shouldContinueAfterSelectingPerson person: ABRecord
) -> Bool
```

Deprecated

Use peoplePickerNavigationController(_:didSelectPerson:) or peoplePickerNavigationController(_:didSelectPerson:property:identifier:) instead.

## Parameters 

`peoplePicker`  

The people-picker navigation controller with which the user interacted.

`person`  

The person the user selected.

## Return Value

true to display the contact and dismiss the picker. false to do nothing.

## See Also

### Responding to User Events

func peoplePickerNavigationController(ABPeoplePickerNavigationController, shouldContinueAfterSelectingPerson: ABRecord, property: ABPropertyID, identifier: ABMultiValueIdentifier) -> Bool

Sent when the user selects one of a person’s properties.

Deprecated

func peoplePickerNavigationControllerDidCancel(ABPeoplePickerNavigationController)

Sent when the user taps Cancel.

func peoplePickerNavigationController(ABPeoplePickerNavigationController, didSelectPerson: ABRecord)

Called after a person has been selected by the user.

func peoplePickerNavigationController(ABPeoplePickerNavigationController, didSelectPerson: ABRecord, property: ABPropertyID, identifier: ABMultiValueIdentifier)

Called after a property has been selected by the user.

