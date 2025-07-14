

- Address Book UI
- ABPeoplePickerNavigationControllerDelegate
-  peoplePickerNavigationController(\_:didSelectPerson:) 

Instance Method

# peoplePickerNavigationController(\_:didSelectPerson:)

Called after a person has been selected by the user.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+

``` source
optional func peoplePickerNavigationController(
    _ peoplePicker: ABPeoplePickerNavigationController,
    didSelectPerson person: ABRecord
)
```

## Parameters 

`peoplePicker`  

The people picker where the selection was made.

`person`  

The selected person record.

## See Also

### Responding to User Events

func peoplePickerNavigationController(ABPeoplePickerNavigationController, shouldContinueAfterSelectingPerson: ABRecord) -> Bool

Sent when the user selects a contact.

Deprecated

func peoplePickerNavigationController(ABPeoplePickerNavigationController, shouldContinueAfterSelectingPerson: ABRecord, property: ABPropertyID, identifier: ABMultiValueIdentifier) -> Bool

Sent when the user selects one of a person’s properties.

Deprecated

func peoplePickerNavigationControllerDidCancel(ABPeoplePickerNavigationController)

Sent when the user taps Cancel.

func peoplePickerNavigationController(ABPeoplePickerNavigationController, didSelectPerson: ABRecord, property: ABPropertyID, identifier: ABMultiValueIdentifier)

Called after a property has been selected by the user.

