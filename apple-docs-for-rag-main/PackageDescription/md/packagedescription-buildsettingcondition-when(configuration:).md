

- PackageDescription
- BuildSettingCondition
-  when(configuration:) 

Type Method

# when(configuration:)

Creates a build setting condition.

SwiftPM 5.7+

``` source
static func when(configuration: BuildConfiguration) -> BuildSettingCondition
```

## Parameters 

`configuration`  

The applicable build configuration for this build setting condition.

## See Also

### Checking for a Build Condition

static func when(platforms: [Platform]) -> BuildSettingCondition

Creates a build setting condition.

static func when(platforms: [Platform]?, configuration: BuildConfiguration?) -> BuildSettingCondition

Creates a build setting condition.

Deprecated

static func when(platforms: [Platform], configuration: BuildConfiguration) -> BuildSettingCondition

Creates a build setting condition.

