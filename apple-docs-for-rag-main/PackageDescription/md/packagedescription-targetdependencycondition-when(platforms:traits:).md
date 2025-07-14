

- PackageDescription
- TargetDependencyCondition
-  when(platforms:traits:) 

Type Method

# when(platforms:traits:)

Creates a target dependency condition.

SwiftPM 6.1+

``` source
static func when(
    platforms: [Platform],
    traits: Set
) -> TargetDependencyCondition?
```

## Parameters 

`platforms`  

The applicable platforms for this target dependency condition.

`traits`  

The applicable traits for this target dependency condition.

