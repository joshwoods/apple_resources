

- LightweightCodeRequirements
-  TeamIdentifierMatchesCurrentProcess 

Structure

# TeamIdentifierMatchesCurrentProcess

A constraint that matches if a process has the same team identifier as the calling process.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct TeamIdentifierMatchesCurrentProcess
```

## Topics

### Initializers

init()

Creates a constraint that matches the current process’s team identifier.

init(Bool)

Creates a constraint that tests whether a process’s team identifier matches the current process’s team identifier.

init(from: any Decoder) throws

Create a new constraint by decoding from the given decoder

### Instance Methods

func encode(to: any Encoder) throws

Encodes this constraint into the given encoder.

## Relationships

### Conforms To

- Decodable
- Encodable
- ProcessConstraint
- Sendable

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

protocol ProcessConstraint

A protocol to which a lightweight code requirement constraint conforms if you can use it in process code requirements.

struct ProcessCodeSigningFlags

A constraint that matches the current code-signing flags of a process.

struct ProcessConstraintBuilder

A custom parameter attribute that constructs process constraints from closures.

