

- Core Spotlight
- CSPerson
-  contactIdentifier 

Instance Property

# contactIdentifier

The identifier for the contact associated with the person.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var contactIdentifier: String? { get set }
```

## Discussion

When you use the contact’s identifier value for the optional contactIdentifier property, it enables a direct way to look up the associated contact.

## See Also

### Accessing person properties

var displayName: String?

A display name for the person.

var handleIdentifier: String

A key that identifies the type of contact property represented by the person object’s handle.

var handles: [String]

An array of contact handles related to the person.

