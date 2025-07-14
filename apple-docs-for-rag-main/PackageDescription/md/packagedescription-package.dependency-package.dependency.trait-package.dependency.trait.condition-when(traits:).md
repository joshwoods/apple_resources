

- PackageDescription
- Package
- 
  - Package
- Package.Dependency
- Package.Dependency.Trait
- Package.Dependency.Trait.Condition
-  when(traits:) 

Type Method

# when(traits:)

Creates a package dependency trait condition.

SwiftPM 6.1+

``` source
static func when(traits: Set) -> Package.Dependency.Trait.Condition?
```

## Parameters 

`traits`  

The set of traits that enable the dependencies trait. If any of the traits are enabled on this package the dependencies trait will be enabled.

