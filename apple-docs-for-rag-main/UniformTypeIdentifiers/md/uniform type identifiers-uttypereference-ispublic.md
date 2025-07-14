

- Uniform Type Identifiers
- UTTypeReference
-  isPublic 

Instance Property

# isPublic

A Boolean value that indicates whether the type is in the public domain.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var isPublic: Bool { get }
```

## Discussion

Types in the public domain have identifiers starting with `public`, and are generally defined by a standards body or by convention. Public types aren’t dynamic.

## See Also

### Obtaining additional type information

var isDeclared: Bool

A Boolean value that indicates whether the system declares the type.

var isDynamic: Bool

A Boolean value that indicates whether the system generates the type.

var referenceURL: URL?

The reference URL for the type.

var version: Int?

The type’s version, if available.

