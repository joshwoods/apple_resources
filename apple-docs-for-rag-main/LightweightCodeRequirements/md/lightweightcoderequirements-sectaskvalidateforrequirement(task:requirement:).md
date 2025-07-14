

- LightweightCodeRequirements
-  SecTaskValidateForRequirement(task:requirement:) 

Function

# SecTaskValidateForRequirement(task:requirement:)

Tests whether a task’s executable satisfies a lightweight code requirement.

Mac Catalyst 17.4+macOS 14.4+

``` source
func SecTaskValidateForRequirement(
    task: SecTask,
    requirement: ProcessCodeRequirement
) throws -> Bool
```

## Parameters 

`task`  

An object that represents the running task.

`requirement`  

The lightweight code requirement to test.

## Return Value

If the requirement matches the process, then `true`; `false` if it doesn’t.

## Discussion

This function throws a value from ConstraintError if it can’t evaluate whether the executable satisfies the lightweight code requirement.

## See Also

### Checking code requirements for running processes

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

struct TeamIdentifierMatchesCurrentProcess

A constraint that matches if a process has the same team identifier as the calling process.

