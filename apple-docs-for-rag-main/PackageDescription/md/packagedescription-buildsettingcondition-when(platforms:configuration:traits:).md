

- PackageDescription
- BuildSettingCondition
-  when(platforms:configuration:traits:) 

Type Method

# when(platforms:configuration:traits:)

Creates a build setting condition.

SwiftPM 6.1+

``` source
static func when(
    platforms: [Platform]? = nil,
    configuration: BuildConfiguration? = nil,
    traits: Set? = nil
) -> BuildSettingCondition
```

## Parameters 

`platforms`  

The applicable platforms for this build setting condition.

`configuration`  

The applicable build configuration for this build setting condition.

`traits`  

The applicable traits for this build setting condition.

