

- PackageDescription
- BuildSettingCondition
-  when(platforms:) 

Type Method

# when(platforms:)

Creates a build setting condition.

SwiftPM 5.7+

``` source
static func when(platforms: [Platform]) -> BuildSettingCondition
```

## Parameters 

`platforms`  

The applicable platforms for this build setting condition.

## See Also

### Checking for a Build Condition

static func when(configuration: BuildConfiguration) -> BuildSettingCondition

Creates a build setting condition.

static func when(platforms: [Platform]?, configuration: BuildConfiguration?) -> BuildSettingCondition

Creates a build setting condition.

Deprecated

static func when(platforms: [Platform], configuration: BuildConfiguration) -> BuildSettingCondition

Creates a build setting condition.

