

- Core Spotlight
- CSPerson
-  handles 

Instance Property

# handles

An array of contact handles related to the person.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var handles: [String] { get }
```

## Discussion

Contact handles can include phone numbers, email addresses, and URLs. For additional contact handles, see Metadata Keys in CNContact.

## See Also

### Accessing person properties

var contactIdentifier: String?

The identifier for the contact associated with the person.

var displayName: String?

A display name for the person.

var handleIdentifier: String

A key that identifies the type of contact property represented by the person object’s handle.

