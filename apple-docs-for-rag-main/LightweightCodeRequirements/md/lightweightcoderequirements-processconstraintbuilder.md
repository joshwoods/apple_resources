

- LightweightCodeRequirements
-  ProcessConstraintBuilder 

Structure

# ProcessConstraintBuilder

A custom parameter attribute that constructs process constraints from closures.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
@resultBuilder
struct ProcessConstraintBuilder
```

## Topics

### Type Methods

static func buildBlock([any ProcessConstraint]...) -> [any ProcessConstraint]

Builds flat array from a variadic set of arrays

static func buildEither(first: [any ProcessConstraint]) -> [any ProcessConstraint]

Produces content for a conditional statement in a multi-statement closure when the condition is true

static func buildEither(second: [any ProcessConstraint]) -> [any ProcessConstraint]

Produces content for a conditional statement in a multi-statement closure when the condition is false

static func buildExpression([any ProcessConstraint]) -> [any ProcessConstraint]

Builds an expression within the builder

static func buildExpression(any ProcessConstraint) -> [any ProcessConstraint]

Builds an expression within the builder

static func buildOptional([any ProcessConstraint]?) -> [any ProcessConstraint]

Produces content for a conditional statement in a multi-statement closure when the condition is true and has no else option.

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

struct TeamIdentifierMatchesCurrentProcess

A constraint that matches if a process has the same team identifier as the calling process.

