

- LightweightCodeRequirements
-  LaunchCodeRequirement 

Structure

# LaunchCodeRequirement

A lightweight code requirement that you use to evaluate the executable for a launching process.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
struct LaunchCodeRequirement
```

## Overview

If you set a `LaunchCodeRequirement` object for a launching process and the executable doesn’t satisfy the requirement, the operating system doesn’t run the process and creates a crash report instead. LaunchCodeRequirement objects can only be built using constraints that conform to the LaunchConstraint protocol. Note that LaunchCodeRequirement are applied to processes. If a launch requests execution of ‘#!’ script, the launch constraint will be applied to the interpreter. For example a script with the following ‘#!’ will apply a launch constraint to bash.

```
```

if the ‘#!’ is instead:

```
```

Then the launch constraint is applied to env.

## Topics

### Initializers

init(ProcessCodeRequirement) throws

Convert a ProcessCodeRequirement to a LaunchCodeRequirement if possible.

init(OnDiskCodeRequirement) throws

Convert a OnDiskCodeRequirement to a LaunchCodeRequirement if possible.

init(from: any Decoder) throws

Create a new instance by decoding from the given decoder

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder

### Type Methods

static func allOf(requirement: () -> [any LaunchConstraint]) throws -> LaunchCodeRequirement

Create a LaunchCodeRequirement that requires matching all of the provided constraints.

static func anyOf(requirement: () -> [any LaunchConstraint]) throws -> LaunchCodeRequirement

Create a LaunchCodeRequirement that requires matching any of the provided constraints.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Sendable

## See Also

### Checking code requirements for launching processes

func SecCodeCheckValidityWithProcessRequirement(code: SecCode, flags: SecCSFlags, requirement: ProcessCodeRequirement) -> ValidationResult

Checks whether the code associated with a running process satisfies a lightweight code requirement.

var launchRequirement: LaunchCodeRequirement?

func allOf(requirement: () -> [any LaunchConstraint]) -> any LaunchConstraint

Creates a constraint that requires a launching process’s executable to satisfy all of the provided constraints.

func anyOf(requirement: () -> [any LaunchConstraint]) -> any LaunchConstraint

Creates a constraint that requires a launching process’s executable to satisfy any of the provided constraints.

protocol LaunchConstraint

A protocol to which a lightweight code requirement constraint conforms if you can use it in launch code requirements.

struct LaunchConstraintBuilder

A custom parameter attribute that constructs launch constraints from closures.

