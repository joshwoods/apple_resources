

- Core Spotlight
- CSPerson
-  handleIdentifier 

Instance Property

# handleIdentifier

A key that identifies the type of contact property represented by the person object’s handle.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var handleIdentifier: String { get }
```

## Discussion

The value of this property is a CNContact property key, such as CNContactPhoneNumbersKey or CNContactEmailAddressesKey.

## See Also

### Accessing person properties

var contactIdentifier: String?

The identifier for the contact associated with the person.

var displayName: String?

A display name for the person.

var handles: [String]

An array of contact handles related to the person.

