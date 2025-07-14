

- LightweightCodeRequirements
-  SecCodeCheckValidityWithProcessRequirement(code:flags:requirement:) 

Function

# SecCodeCheckValidityWithProcessRequirement(code:flags:requirement:)

Checks whether the code associated with a running process satisfies a lightweight code requirement.

Mac Catalyst 18.0+macOS 15.0+

``` source
func SecCodeCheckValidityWithProcessRequirement(
    code: SecCode,
    flags: SecCSFlags,
    requirement: ProcessCodeRequirement
) -> ValidationResult
```

## Discussion

Returns a validation result which indicates whether the code signature is valid, whether it matches the requirement, and if not one of those two, then why not.

## See Also

### Checking code requirements for launching processes

var launchRequirement: LaunchCodeRequirement?

struct LaunchCodeRequirement

A lightweight code requirement that you use to evaluate the executable for a launching process.

func allOf(requirement: () -> [any LaunchConstraint]) -> any LaunchConstraint

Creates a constraint that requires a launching process’s executable to satisfy all of the provided constraints.

func anyOf(requirement: () -> [any LaunchConstraint]) -> any LaunchConstraint

Creates a constraint that requires a launching process’s executable to satisfy any of the provided constraints.

protocol LaunchConstraint

A protocol to which a lightweight code requirement constraint conforms if you can use it in launch code requirements.

struct LaunchConstraintBuilder

A custom parameter attribute that constructs launch constraints from closures.

