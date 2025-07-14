

- Address Book UI
- ABPeoplePickerNavigationController
-  displayedProperties Deprecated

Instance Property

# displayedProperties

The properties (such as name or telephone number) the picker displays when it shows a person.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var displayedProperties: [NSNumber]? { get set }
```

Deprecated

Use CNContactPickerViewController instead.

## Discussion

Objects in the array are instances of NSNumber that represent ABPropertyID values.

The name property is always displayed if available.

To have the picker display a single property for the person displayed, such as the telephone number, set `displayedProperties` to an array with a single value, such as `kABPersonPhoneProperty`.

