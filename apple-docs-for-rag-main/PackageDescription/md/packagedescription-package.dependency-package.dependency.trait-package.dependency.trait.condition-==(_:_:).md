

- PackageDescription
- Package
- 
  - Package
- Package.Dependency
- Package.Dependency.Trait
- Package.Dependency.Trait.Condition
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two values are equal.

SwiftPM 6.1+

``` source
static func == (a: Package.Dependency.Trait.Condition, b: Package.Dependency.Trait.Condition) -> Bool
```

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Equality is the inverse of inequality. For any values `a` and `b`, `a == b` implies that `a != b` is `false`.

