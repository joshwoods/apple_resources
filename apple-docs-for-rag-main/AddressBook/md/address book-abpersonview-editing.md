

- Address Book
- ABPersonView
-  editing 

Instance Property

# editing

A Boolean value that indicates whether the person view is in editing mode.

macOS 10.7+

``` source
@MainActor
var editing: Bool { get set }
```

## Discussion

In editing mode, the person view displays additional controls to let the user change the contact’s information.

## See Also

### Working with Person Views

var person: ABPerson!

The contact record being displayed.

var shouldShowLinkedPeople: Bool

Indicates whether the person view should display data from person records that are linked with the person record being displayed.

