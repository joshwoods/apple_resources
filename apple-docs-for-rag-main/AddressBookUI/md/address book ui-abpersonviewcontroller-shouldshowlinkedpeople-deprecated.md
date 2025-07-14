

- Address Book UI
- ABPersonViewController
-  shouldShowLinkedPeople Deprecated

Instance Property

# shouldShowLinkedPeople

Indicates whether the person view should display data from person records that are linked with the person record being displayed.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var shouldShowLinkedPeople: Bool { get set }
```

Deprecated

Use CNContactViewController instead.

## Discussion

Linked records represent the same actual person. They often come from different sources, but may also come from the same source.

## See Also

### Displaying Person Properties

var displayedPerson: ABRecord

The person displayed by the person view.

Deprecated

var displayedProperties: [NSNumber]?

Identifies the set of properties (such as name or telephone number) of displayedPerson the receiver displays.

Deprecated

