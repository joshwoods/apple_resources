

- Address Book UI
- ABNewPersonViewController
-  displayedPerson Deprecated

Instance Property

# displayedPerson

Optional. Specifies the person properties that the new-person view controller pre-fills in its views.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var displayedPerson: ABRecord? { get set }
```

Deprecated

Use contact instead.

## Discussion

When this property has no person properties, the new-person view controller does not pre-fill properties in its views.

