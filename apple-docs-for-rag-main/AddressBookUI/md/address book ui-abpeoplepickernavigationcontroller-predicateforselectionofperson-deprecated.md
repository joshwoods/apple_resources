

- Address Book UI
- ABPeoplePickerNavigationController
-  predicateForSelectionOfPerson Deprecated

Instance Property

# predicateForSelectionOfPerson

Optionally determines if a selected person should be returned to the app or displayed.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@NSCopying @MainActor
var predicateForSelectionOfPerson: NSPredicate? { get set }
```

Deprecated

Use CNContactPickerViewController instead.

## Discussion

If the predicate evaluates to true for the selected person, the selected person is returned to the app. If the predicate evaluates to false, the selected person is displayed.

If this property is `nil`, the person is returned to the app if the delegate implements peoplePickerNavigationController(_:didSelectPerson:), and the person is displayed if the delegate implements peoplePickerNavigationController(_:didSelectPerson:property:identifier:).

## See Also

### Customizing Display and Selection

var predicateForEnablingPerson: NSPredicate?

Optionally determines if a person can be selected.

Deprecated

var predicateForSelectionOfProperty: NSPredicate?

Optionally determines if a selected property should be returned to the app or if the default action for the property should be performed

Deprecated

