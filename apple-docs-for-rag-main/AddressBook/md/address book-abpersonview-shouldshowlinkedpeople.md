

- Address Book
- ABPersonView
-  shouldShowLinkedPeople 

Instance Property

# shouldShowLinkedPeople

Indicates whether the person view should display data from person records that are linked with the person record being displayed.

macOS 10.8+

``` source
@MainActor
var shouldShowLinkedPeople: Bool { get set }
```

## Discussion

Linked records represent the same actual person, and typically come from different sources.

## See Also

### Working with Person Views

var editing: Bool

A Boolean value that indicates whether the person view is in editing mode.

var person: ABPerson!

The contact record being displayed.

