

- Address Book UI
- ABUnknownPersonViewController
-  displayedPerson Deprecated

Instance Property

# displayedPerson

Specifies a person record whose properties are displayed by the view controller.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var displayedPerson: ABRecord { get set }
```

Deprecated

Use CNContactViewController instead.

## Discussion

All the properties of `displayedPerson` are displayed by the view controller.

## See Also

### Displaying Person Properties

var alternateName: String?

Provides a value that is displayed instead of the first and last name.

Deprecated

var message: String?

Text displayed below alternateName.

Deprecated

