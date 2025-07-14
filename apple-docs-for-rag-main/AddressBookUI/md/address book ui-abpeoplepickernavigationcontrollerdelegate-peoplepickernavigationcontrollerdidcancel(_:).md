

- Address Book UI
- ABPeoplePickerNavigationControllerDelegate
-  peoplePickerNavigationControllerDidCancel(\_:) 

Instance Method

# peoplePickerNavigationControllerDidCancel(\_:)

Sent when the user taps Cancel.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+

``` source
optional func peoplePickerNavigationControllerDidCancel(_ peoplePicker: ABPeoplePickerNavigationController)
```

## Parameters 

`peoplePicker`  

The people-picker navigation controller with which the user interacted.

## Discussion

If the delegate does not implement this method, the people picker will dismiss itself when the user taps cancel.

### Special Considerations

Prior to iOS 8, the delegate was responsible for dismissing the people picker and this method was required.

## See Also

### Responding to User Events

func peoplePickerNavigationController(ABPeoplePickerNavigationController, shouldContinueAfterSelectingPerson: ABRecord) -> Bool

Sent when the user selects a contact.

Deprecated

func peoplePickerNavigationController(ABPeoplePickerNavigationController, shouldContinueAfterSelectingPerson: ABRecord, property: ABPropertyID, identifier: ABMultiValueIdentifier) -> Bool

Sent when the user selects one of a person’s properties.

Deprecated

func peoplePickerNavigationController(ABPeoplePickerNavigationController, didSelectPerson: ABRecord)

Called after a person has been selected by the user.

func peoplePickerNavigationController(ABPeoplePickerNavigationController, didSelectPerson: ABRecord, property: ABPropertyID, identifier: ABMultiValueIdentifier)

Called after a property has been selected by the user.

