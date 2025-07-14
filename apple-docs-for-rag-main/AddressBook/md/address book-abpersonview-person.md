

- Address Book
- ABPersonView
-  person 

Instance Property

# person

The contact record being displayed.

macOS 10.7+

``` source
@MainActor
var person: ABPerson! { get set }
```

## Discussion

If the value of this property is `nil`, the view displays a special empty-selection UI.

An exception is raised if the value of this property comes from a shared instance of the address book database. To prevent this, use the addressBook method of ABAddressBook rather than the shared() method.

## See Also

### Working with Person Views

var editing: Bool

A Boolean value that indicates whether the person view is in editing mode.

var shouldShowLinkedPeople: Bool

Indicates whether the person view should display data from person records that are linked with the person record being displayed.

