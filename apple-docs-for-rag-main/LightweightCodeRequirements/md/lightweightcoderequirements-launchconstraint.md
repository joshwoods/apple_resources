

- LightweightCodeRequirements
-  LaunchConstraint 

Protocol

# LaunchConstraint

A protocol to which a lightweight code requirement constraint conforms if you can use it in launch code requirements.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
protocol LaunchConstraint : Decodable, Encodable, Sendable
```

## Relationships

### Inherits From

- Decodable
- Encodable
- Sendable

### Conforming Types

- CodeDirectoryHash
- EntitlementsQuery
- InfoPlistHash
- IsInitProcess
- IsSIPProtected
- PlatformType
- ProcessCodeSigningFlags
- SigningIdentifier
- TeamIdentifier
- ValidationCategory

## See Also

### Checking code requirements for launching processes

func SecCodeCheckValidityWithProcessRequirement(code: SecCode, flags: SecCSFlags, requirement: ProcessCodeRequirement) -> ValidationResult

Checks whether the code associated with a running process satisfies a lightweight code requirement.

var launchRequirement: LaunchCodeRequirement?

struct LaunchCodeRequirement

A lightweight code requirement that you use to evaluate the executable for a launching process.

func allOf(requirement: () -> [any LaunchConstraint]) -> any LaunchConstraint

Creates a constraint that requires a launching process’s executable to satisfy all of the provided constraints.

func anyOf(requirement: () -> [any LaunchConstraint]) -> any LaunchConstraint

Creates a constraint that requires a launching process’s executable to satisfy any of the provided constraints.

struct LaunchConstraintBuilder

A custom parameter attribute that constructs launch constraints from closures.

