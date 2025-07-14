

- Contacts UI
- CNContactPickerViewController
-  predicateForEnablingContact 

Instance Property

# predicateForEnablingContact

A predicate to determine the contact selectability in the list of contacts.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@NSCopying @MainActor
var predicateForEnablingContact: NSPredicate? { get set }
```

## Discussion

You can set a value for this property to determine which contact should become selectable, such as `emailAddresses.@count > 0` to enable all the contacts that have an email address to become selectable. If no predicate is set for this property, all contacts become selectable. To learn about predicate syntax, see NSPredicate.

## See Also

### Predicates For Selecting Contacts

var predicateForSelectionOfContact: NSPredicate?

A predicate to control the return of the selected contact.

var predicateForSelectionOfProperty: NSPredicate?

A predicate to control the properties of the selected contact.

