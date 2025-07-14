

- PackageDescription
- Package
- Package.Dependency
- Package.Dependency.Trait
-  trait(name:condition:) 

Type Method

# trait(name:condition:)

Initializes a new enabled trait.

SwiftPM 6.1+

``` source
static func trait(
    name: String,
    condition: Package.Dependency.Trait.Condition? = nil
) -> Package.Dependency.Trait
```

## Parameters 

`name`  

The name of the enabled trait.

`condition`  

The condition under which the trait is enabled.

