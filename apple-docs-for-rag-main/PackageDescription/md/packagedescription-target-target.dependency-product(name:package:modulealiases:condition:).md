

- PackageDescription
- Target
- Target.Dependency
-  product(name:package:moduleAliases:condition:) 

Type Method

# product(name:package:moduleAliases:condition:)

Creates a target dependency on a product from a package dependency.

SwiftPM 5.7+

``` source
static func product(
    name: String,
    package: String,
    moduleAliases: [String : String]? = nil,
    condition: TargetDependencyCondition? = nil
) -> Target.Dependency
```

## Parameters 

`name`  

The name of the product.

`package`  

The name of the package.

`moduleAliases`  

The module aliases for targets in the product.

`condition`  

A condition that limits the application of the target dependency. For example, only apply a dependency for a specific platform.

## Return Value

A `Target.Dependency` instance.

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

