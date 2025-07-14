

- PackageDescription
- Target
- Target.Dependency
-  init(stringLiteral:) 

Initializer

# init(stringLiteral:)

Creates a target dependency instance with the given value.

``` source
init(stringLiteral value: String)
```

## Parameters 

`value`  

A string literal.

## See Also

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

init(extendedGraphemeClusterLiteral: Self.StringLiteralType)

init(unicodeScalarLiteral: Self.ExtendedGraphemeClusterLiteralType)

