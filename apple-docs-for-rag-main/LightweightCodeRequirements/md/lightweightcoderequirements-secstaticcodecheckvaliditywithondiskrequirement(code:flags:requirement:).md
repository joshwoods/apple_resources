

- LightweightCodeRequirements
-  SecStaticCodeCheckValidityWithOnDiskRequirement(code:flags:requirement:) 

Function

# SecStaticCodeCheckValidityWithOnDiskRequirement(code:flags:requirement:)

Checks whether static code on disk satisfies a lightweight code requirement.

Mac Catalyst 17.4+macOS 14.4+

``` source
func SecStaticCodeCheckValidityWithOnDiskRequirement(
    code: SecStaticCode,
    flags: SecCSFlags,
    requirement: OnDiskCodeRequirement
) -> ValidationResult
```

## Discussion

Returns a validation result which indicates whether the code signature is valid, whether it matches the requirement, and if not one of those two, then why not.

## See Also

### Checking code requirements for code files on disk

func SecCodeCheckValidityWithOnDiskRequirement(code: SecCode, flags: SecCSFlags, requirement: OnDiskCodeRequirement) -> ValidationResult

Checks whether code on disk satisfies a lightweight code requirement.

struct ValidationResult

A structure that represents the result of testing a lightweight code requirement.

struct OnDiskCodeRequirement

A lightweight code requirement that you use to evaluate a code file on disk.

func allOf(requirement: () -> [any OnDiskConstraint]) -> any OnDiskConstraint

Creates a constraint that requires code on disk to satisfy all of the provided constraints.

func anyOf(requirement: () -> [any OnDiskConstraint]) -> any OnDiskConstraint

Creates a constraint that requires code on disk to satisfy any of the provided constraints.

protocol OnDiskConstraint

A protocol to which a lightweight code requirement constraint conforms if you can use it in on-disk code requirements.

struct OnDiskCodeSigningFlags

A constraint that tests the code-signing flags of a code file on disk.

struct OnDiskConstraintBuilder

A custom parameter attribute that constructs on-disk constraints from closures.

