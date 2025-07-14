

- Uniform Type Identifiers
- UTTypeReference
-  isDynamic 

Instance Property

# isDynamic

A Boolean value that indicates whether the system generates the type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var isDynamic: Bool { get }
```

## Discussion

The system recognizes dynamic types, but they may not be directly declared or claimed by an app. The system returns dynamic types when it encounters a file whose metadata doesn’t have a corresponding type known to the system.

The system either declares a type or dynamically generates a type, but not both.

## See Also

### Obtaining additional type information

var isDeclared: Bool

A Boolean value that indicates whether the system declares the type.

var isPublic: Bool

A Boolean value that indicates whether the type is in the public domain.

var referenceURL: URL?

The reference URL for the type.

var version: Int?

The type’s version, if available.

