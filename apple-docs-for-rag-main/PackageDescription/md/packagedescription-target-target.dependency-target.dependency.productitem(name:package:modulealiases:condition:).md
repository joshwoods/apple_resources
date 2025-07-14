

- PackageDescription
- Target
- Target.Dependency
-  Target.Dependency.productItem(name:package:moduleAliases:condition:) 

Case

# Target.Dependency.productItem(name:package:moduleAliases:condition:)

A dependency on a product.

``` source
case productItem(
    name: String,
    package: String?,
    moduleAliases: [String : String]?,
    condition: TargetDependencyCondition?
)
```

## Parameters 

`name`  

The name of the product.

`package`  

The name of the package.

`moduleAlias`  

The module aliases for targets in the product.

`condition`  

A condition that limits the application of the target dependency. For example, only apply a dependency for a specific platform.

