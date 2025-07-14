

- LightweightCodeRequirements
-  ProcessCodeRequirement 

Structure

# ProcessCodeRequirement

A lightweight code requirement that you use to evaluate a running process.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
struct ProcessCodeRequirement
```

## Overview

ProcessCodeRequirement objects can only be built using constraints that conform to the ProcessConstraint protocol.

## Topics

### Initializers

init(OnDiskCodeRequirement) throws

Convert an OnDiskCodeRequirement to a ProcessCodeRequirement if possible.

init(LaunchCodeRequirement) throws

Convert a LaunchCodeRequirement to a ProcessCodeRequirement if possible.

init(from: any Decoder) throws

Create a new instance by decoding from the given decoder

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder

### Type Methods

static func allOf(requirement: () -> [any ProcessConstraint]) throws -> ProcessCodeRequirement

Create a ProcessCodeRequirement that requires matching all of the provided constraints.

static func anyOf(requirement: () -> [any ProcessConstraint]) throws -> ProcessCodeRequirement

Create a ProcessCodeRequirement that requires matching any of the provided constraints.

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

### Checking code requirements for running processes

func SecTaskValidateForRequirement(task: SecTask, requirement: ProcessCodeRequirement) throws -> Bool

Tests whether a task’s executable satisfies a lightweight code requirement.

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

