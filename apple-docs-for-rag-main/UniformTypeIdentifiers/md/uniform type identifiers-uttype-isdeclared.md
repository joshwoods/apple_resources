

- Uniform Type Identifiers
- UTType
-  isDeclared 

Instance Property

# isDeclared

A Boolean value that indicates whether the system declares the type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var isDeclared: Bool { get }
```

## Discussion

The system either declares a type or dynamically generates a type, but not both.

## See Also

### Obtaining additional type information

var isDynamic: Bool

A Boolean value that indicates whether the system generates the type.

var isPublic: Bool

A Boolean value that indicates whether the type is in the public domain.

var referenceURL: URL?

The reference URL for the type.

var version: Int?

The type’s version, if available.

