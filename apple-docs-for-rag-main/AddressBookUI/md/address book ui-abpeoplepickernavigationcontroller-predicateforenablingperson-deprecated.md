

- Address Book UI
- ABPeoplePickerNavigationController
-  predicateForEnablingPerson Deprecated

Instance Property

# predicateForEnablingPerson

Optionally determines if a person can be selected.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@NSCopying @MainActor
var predicateForEnablingPerson: NSPredicate? { get set }
```

Deprecated

Use CNContactPickerViewController instead.

## Discussion

If not set, all persons are selectable.

## See Also

### Customizing Display and Selection

var predicateForSelectionOfPerson: NSPredicate?

Optionally determines if a selected person should be returned to the app or displayed.

Deprecated

var predicateForSelectionOfProperty: NSPredicate?

Optionally determines if a selected property should be returned to the app or if the default action for the property should be performed

Deprecated

