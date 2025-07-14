

- PackageDescription
- Target
- Target.Dependency
-  Target.Dependency.byNameItem(name:condition:) 

Case

# Target.Dependency.byNameItem(name:condition:)

A by-name dependency on either a target or a product.

``` source
case byNameItem(
    name: String,
    condition: TargetDependencyCondition?
)
```

## Parameters 

`name`  

The name of the dependency, either a target or a product.

`condition`  

A condition that limits the application of the target dependency. For example, only apply a dependency for a specific platform.

