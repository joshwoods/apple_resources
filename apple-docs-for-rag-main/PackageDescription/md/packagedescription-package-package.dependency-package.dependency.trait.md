

- PackageDescription
- Package
- Package.Dependency
-  Package.Dependency.Trait 

Structure

# Package.Dependency.Trait

A struct representing an enabled trait of a dependency.

SwiftPM 6.1+

``` source
struct Trait
```

## Topics

### Structures

struct Condition

A condition that limits the application of a dependencies trait.

### Operators

static func == (Package.Dependency.Trait, Package.Dependency.Trait) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(name: String, condition: Package.Dependency.Trait.Condition?)

Initializes a new enabled trait.

init(stringLiteral: StringLiteralType)

Creates an instance initialized to the given string value.

### Instance Properties

var condition: Package.Dependency.Trait.Condition?

The condition under which the trait is enabled.

var hashValue: Int

The hash value.

var name: String

The name of the enabled trait.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias ExtendedGraphemeClusterLiteralType

A type that represents an extended grapheme cluster literal.

typealias StringLiteralType

A type that represents a string literal.

typealias UnicodeScalarLiteralType

A type that represents a Unicode scalar literal.

### Type Properties

static let defaults: Package.Dependency.Trait

Enables all default traits of a package.

### Type Methods

static func trait(name: String, condition: Package.Dependency.Trait.Condition?) -> Package.Dependency.Trait

Initializes a new enabled trait.

### Default Implementations

Equatable Implementations

ExpressibleByExtendedGraphemeClusterLiteral Implementations

ExpressibleByStringLiteral Implementations

## Relationships

### Conforms To

- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Hashable
- Sendable

