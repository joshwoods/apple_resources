

- Address Book UI
- ABPeoplePickerNavigationController
-  predicateForSelectionOfProperty Deprecated

Instance Property

# predicateForSelectionOfProperty

Optionally determines if a selected property should be returned to the app or if the default action for the property should be performed

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@NSCopying @MainActor
var predicateForSelectionOfProperty: NSPredicate? { get set }
```

Deprecated

Use CNContactPickerViewController instead.

## Discussion

If the predicate evaluates to true, the selected property is returned to the app. If the predicate evaluates to false, the default action for the property is performed.

If this property is `nil`, the selected property is returned to the app if the delegate implements peoplePickerNavigationController(_:didSelectPerson:property:identifier:).

## See Also

### Customizing Display and Selection

var predicateForEnablingPerson: NSPredicate?

Optionally determines if a person can be selected.

Deprecated

var predicateForSelectionOfPerson: NSPredicate?

Optionally determines if a selected person should be returned to the app or displayed.

Deprecated

