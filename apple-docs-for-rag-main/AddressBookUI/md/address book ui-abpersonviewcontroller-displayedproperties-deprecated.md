

- Address Book UI
- ABPersonViewController
-  displayedProperties Deprecated

Instance Property

# displayedProperties

Identifies the set of properties (such as name or telephone number) of displayedPerson the receiver displays.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var displayedProperties: [NSNumber]? { get set }
```

Deprecated

Use CNContactViewController instead.

## Discussion

The default value of this property is `NULL`.

Name properties are always displayed.

The properties are specified using an array of NSNumber objects representing ABPropertyID values.

To have the receiver display a single property for displayedPerson, such as telephone number, set `displayedProperties` to an array with a single value, such as `kABPersonPhoneProperty`.

## See Also

### Displaying Person Properties

var displayedPerson: ABRecord

The person displayed by the person view.

Deprecated

var shouldShowLinkedPeople: Bool

Indicates whether the person view should display data from person records that are linked with the person record being displayed.

Deprecated

