

- LightweightCodeRequirements
-  ProcessCodeSigningFlags 

Structure

# ProcessCodeSigningFlags

A constraint that matches the current code-signing flags of a process.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
struct ProcessCodeSigningFlags
```

## Topics

### Structures

struct ValueSet

Code signing flags that can be set on a process

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Type Aliases

typealias DataType

The basic input data type for this constraint: `ProcessCodeSigningFlags.ValueSet`

typealias OutType

The type of this constraint: ProcessCodeSigningFlags

### Type Methods

static func isSuperset(of: ProcessCodeSigningFlags.DataType) -> ProcessCodeSigningFlags.OutType

Matches when the code signing flags on the process are a superset of the specified flags.

## Relationships

### Conforms To

- Decodable
- Encodable
- LaunchConstraint
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

struct ProcessConstraintBuilder

A custom parameter attribute that constructs process constraints from closures.

struct TeamIdentifierMatchesCurrentProcess

A constraint that matches if a process has the same team identifier as the calling process.

