

- Uniform Type Identifiers
- UTType
-  referenceURL 

Instance Property

# referenceURL

The reference URL for the type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var referenceURL: URL? { get }
```

## Discussion

A reference URL is a human-readable document that describes a type. Most types don’t specify reference URLs.

Warning

The system doesn’t validate the URL, nor does it guarantee its scheme or structure.

## See Also

### Obtaining additional type information

var isDeclared: Bool

A Boolean value that indicates whether the system declares the type.

var isDynamic: Bool

A Boolean value that indicates whether the system generates the type.

var isPublic: Bool

A Boolean value that indicates whether the type is in the public domain.

var version: Int?

The type’s version, if available.

