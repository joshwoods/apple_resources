

- Address Book UI
- ABPeoplePickerNavigationController
-  peoplePickerDelegate Deprecated

Instance Property

# peoplePickerDelegate

The people-picker navigation controller delegate.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
unowned(unsafe) var peoplePickerDelegate: (any ABPeoplePickerNavigationControllerDelegate)? { get set }
```

Deprecated

Use delegate instead.

## Discussion

Optional to get the selected contact, selected property or cancellation of the people picker.

## See Also

### Responding to View Controller Interactions

protocol ABPeoplePickerNavigationControllerDelegate

The `ABPeoplePickerNavigationControllerDelegate` protocol describes the interface ABPeoplePickerNavigationController delegates must adopt to respond to people-picker user events.

Deprecated

