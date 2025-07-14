

- LightweightCodeRequirements
-  ProcessConstraint 

Protocol

# ProcessConstraint

A protocol to which a lightweight code requirement constraint conforms if you can use it in process code requirements.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
protocol ProcessConstraint : Decodable, Encodable, Sendable
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
- TeamIdentifierMatchesCurrentProcess
- ValidationCategory

## See Also

### Checking code requirements for running processes

func SecTaskValidateForRequirement(task: SecTask, requirement: ProcessCodeRequirement) throws -> Bool

Tests whether a task’s executable satisfies a lightweight code requirement.

struct ProcessCodeRequirement

A lightweight code requirement that you use to evaluate a running process.

func allOf(requirement: () -> [any ProcessConstraint]) -> any ProcessConstraint

Creates a constraint that requires a running process’s executable to satisfy all of the provided constraints.

func anyOf(requirement: () -> [any ProcessConstraint]) -> any ProcessConstraint

Creates a constraint that requires a running process’s executable to satisfy any of the provided constraints.

struct ProcessCodeSigningFlags

A constraint that matches the current code-signing flags of a process.

struct ProcessConstraintBuilder

A custom parameter attribute that constructs process constraints from closures.

struct TeamIdentifierMatchesCurrentProcess

A constraint that matches if a process has the same team identifier as the calling process.

