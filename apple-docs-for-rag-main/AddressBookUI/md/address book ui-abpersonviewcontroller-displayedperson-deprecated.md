

- Address Book UI
- ABPersonViewController
-  displayedPerson Deprecated

Instance Property

# displayedPerson

The person displayed by the person view.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var displayedPerson: ABRecord { get set }
```

Deprecated

Use CNContactViewController instead.

## Discussion

The receiver displays the properties of this person record that are present in displayedProperties.

## See Also

### Displaying Person Properties

var displayedProperties: [NSNumber]?

Identifies the set of properties (such as name or telephone number) of displayedPerson the receiver displays.

Deprecated

var shouldShowLinkedPeople: Bool

Indicates whether the person view should display data from person records that are linked with the person record being displayed.

Deprecated

