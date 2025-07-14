

- PackageDescription
- Target
-  Target.Dependency 

Enumeration

# Target.Dependency

The different types of a target’s dependency on another entity.

``` source
enum Dependency
```

## Topics

### Creating a Target Dependency

static func product(name: String, package: String, condition: TargetDependencyCondition?) -> Target.Dependency

Creates a target dependency on a product from a package dependency.

Deprecated

static func product(name: String, package: String?) -> Target.Dependency

Creates a dependency on a product from a package dependency.

Deprecated

static func product(name: String, package: String) -> Target.Dependency

Creates a dependency on a product from a package dependency.

Deprecated

static func product(name: String, package: String, moduleAliases: [String : String]?, condition: TargetDependencyCondition?) -> Target.Dependency

Creates a target dependency on a product from a package dependency.

static func target(name: String, condition: TargetDependencyCondition?) -> Target.Dependency

Creates a dependency on a target in the same package.

static func target(name: String) -> Target.Dependency

Creates a dependency on a target in the same package.

Deprecated

static func byName(name: String, condition: TargetDependencyCondition?) -> Target.Dependency

Creates a dependency that resolves to either a target or a product with the specified name.

static func byName(name: String) -> Target.Dependency

Creates a dependency that resolves to either a target or a product with the specified name.

Deprecated

struct TargetDependencyCondition

A condition that limits the application of a target’s dependency.

init(stringLiteral: String)

Creates a target dependency instance with the given value.

init(extendedGraphemeClusterLiteral: Self.StringLiteralType)

init(unicodeScalarLiteral: Self.ExtendedGraphemeClusterLiteralType)

### Identifying related types

typealias ExtendedGraphemeClusterLiteralType

A type that represents an extended grapheme cluster literal.

typealias StringLiteralType

A type that represents a string literal.

typealias UnicodeScalarLiteralType

A type that represents a Unicode scalar literal.

### Enumeration Cases

case byNameItem(name: String, condition: TargetDependencyCondition?)

A by-name dependency on either a target or a product.

case productItem(name: String, package: String?, moduleAliases: [String : String]?, condition: TargetDependencyCondition?)

A dependency on a product.

case targetItem(name: String, condition: TargetDependencyCondition?)

A dependency on a target.

### Type Methods

static func productItem(name: String, package: String?, condition: TargetDependencyCondition?) -> Target.DependencyDeprecated

### Default Implementations

ExpressibleByExtendedGraphemeClusterLiteral Implementations

ExpressibleByStringLiteral Implementations

ExpressibleByUnicodeScalarLiteral Implementations

## Relationships

### Conforms To

- Copyable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Sendable

## See Also

### Declaring a Dependency Target

var dependencies: [Target.Dependency]

The target’s dependencies on other entities inside or outside the package.

struct TargetDependencyCondition

A condition that limits the application of a target’s dependency.

