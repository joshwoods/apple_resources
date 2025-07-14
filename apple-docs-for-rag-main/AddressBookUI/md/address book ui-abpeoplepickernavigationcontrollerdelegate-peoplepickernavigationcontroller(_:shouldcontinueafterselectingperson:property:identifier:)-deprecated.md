

- Address Book UI
- ABPeoplePickerNavigationControllerDelegate
-  peoplePickerNavigationController(\_:shouldContinueAfterSelectingPerson:property:identifier:) Deprecated

Instance Method

# peoplePickerNavigationController(\_:shouldContinueAfterSelectingPerson:property:identifier:)

Sent when the user selects one of a person’s properties.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
optional func peoplePickerNavigationController(
    _ peoplePicker: ABPeoplePickerNavigationController,
    shouldContinueAfterSelectingPerson person: ABRecord,
    property: ABPropertyID,
    identifier: ABMultiValueIdentifier
) -> Bool
```

Deprecated

Use peoplePickerNavigationController(_:didSelectPerson:) or peoplePickerNavigationController(_:didSelectPerson:property:identifier:) instead.

## Parameters 

`peoplePicker`  

The people-picker navigation controller with which the user interacted.

`person`  

The person whose contact information item the user selected.

`property`  

The property the user selected.

`identifier`  

The identifier for the value the user selected if `property` is a multivalue property; otherwise, `kABMultiValueInvalidIdentifier`.

## Return Value

true to perform the action for the property selected and dismiss the picker. false to show the person in the picker.

## Discussion

This method is called with an identifier. If you need an index, use the ABMultiValueGetIndexForIdentifier(_:_:) function to get the corresponding index.

## See Also

### Responding to User Events

func peoplePickerNavigationController(ABPeoplePickerNavigationController, shouldContinueAfterSelectingPerson: ABRecord) -> Bool

Sent when the user selects a contact.

Deprecated

func peoplePickerNavigationControllerDidCancel(ABPeoplePickerNavigationController)

Sent when the user taps Cancel.

func peoplePickerNavigationController(ABPeoplePickerNavigationController, didSelectPerson: ABRecord)

Called after a person has been selected by the user.

func peoplePickerNavigationController(ABPeoplePickerNavigationController, didSelectPerson: ABRecord, property: ABPropertyID, identifier: ABMultiValueIdentifier)

Called after a property has been selected by the user.

