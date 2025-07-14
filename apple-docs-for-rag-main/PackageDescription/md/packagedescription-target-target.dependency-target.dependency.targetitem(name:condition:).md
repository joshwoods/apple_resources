

- PackageDescription
- Target
- Target.Dependency
-  Target.Dependency.targetItem(name:condition:) 

Case

# Target.Dependency.targetItem(name:condition:)

A dependency on a target.

``` source
case targetItem(
    name: String,
    condition: TargetDependencyCondition?
)
```

## Parameters 

`name`  

The name of the target.

`condition`  

A condition that limits the application of the target dependency. For example, only apply a dependency for a specific platform.

