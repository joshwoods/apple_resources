

- PackageDescription
- TargetDependencyCondition
-  when(platforms:) 

Type Method

# when(platforms:)

Creates a target dependency condition.

SwiftPM 5.7+

``` source
static func when(platforms: [Platform]) -> TargetDependencyCondition?
```

## Parameters 

`platforms`  

The applicable platforms for this target dependency condition.

## See Also

### Creating a Dependency Condition

static func when(platforms: [Platform]?) -> TargetDependencyCondition

Creates a target dependency condition.

Deprecated

