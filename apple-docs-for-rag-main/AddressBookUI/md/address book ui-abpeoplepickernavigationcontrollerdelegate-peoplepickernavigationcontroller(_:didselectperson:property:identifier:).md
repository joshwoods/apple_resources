

- Address Book UI
- ABPeoplePickerNavigationControllerDelegate
-  peoplePickerNavigationController(\_:didSelectPerson:property:identifier:) 

Instance Method

# peoplePickerNavigationController(\_:didSelectPerson:property:identifier:)

Called after a property has been selected by the user.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+

``` source
optional func peoplePickerNavigationController(
    _ peoplePicker: ABPeoplePickerNavigationController,
    didSelectPerson person: ABRecord,
    property: ABPropertyID,
    identifier: ABMultiValueIdentifier
)
```

## Parameters 

`peoplePicker`  

The people picker where the selection was made.

`person`  

The selected person record.

`property`  

The selected property.

`identifier`  

The selected property identifier.

## Discussion

This method is called with an identifier. If you need an index, use the ABMultiValueGetIndexForIdentifier(_:_:) function to get the corresponding index.

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

func peoplePickerNavigationController(ABPeoplePickerNavigationController, didSelectPerson: ABRecord)

Called after a person has been selected by the user.

