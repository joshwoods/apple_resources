

- Address Book UI
- ABUnknownPersonViewController
-  alternateName Deprecated

Instance Property

# alternateName

Provides a value that is displayed instead of the first and last name.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var alternateName: String? { get set }
```

Deprecated

Use CNContactViewController instead.

## Discussion

The alternate name is only for display. It is not saved if this contact is added to the address book database.

## See Also

### Displaying Person Properties

var message: String?

Text displayed below alternateName.

Deprecated

var displayedPerson: ABRecord

Specifies a person record whose properties are displayed by the view controller.

Deprecated

