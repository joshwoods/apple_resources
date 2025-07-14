

- PackageDescription
- Package
- Package.Dependency
- Package.Dependency.Trait
-  init(name:condition:) 

Initializer

# init(name:condition:)

Initializes a new enabled trait.

SwiftPM 6.1+

``` source
init(
    name: String,
    condition: Package.Dependency.Trait.Condition? = nil
)
```

## Parameters 

`name`  

The name of the enabled trait.

`condition`  

The condition under which the trait is enabled.

