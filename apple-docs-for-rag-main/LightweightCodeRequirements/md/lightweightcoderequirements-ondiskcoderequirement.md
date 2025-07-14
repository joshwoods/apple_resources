

- LightweightCodeRequirements
-  OnDiskCodeRequirement 

Structure

# OnDiskCodeRequirement

A lightweight code requirement that you use to evaluate a code file on disk.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
struct OnDiskCodeRequirement
```

## Overview

OnDiskCodeRequirement objects can only be built using constraints that conform to the OnDiskConstraint protocol. Specifically OnDiskCodeRequirement objects will be matched against a SecStaticCodeRef. A SecStaticCodeRef may reference any of the following:

- The main executable of a bundle

- A specific file on disk

- The region of a Mach-O pertaining to a specific architecture (e.g. x86_64, arm64, arm64e).

## Topics

### Initializers

init(LaunchCodeRequirement) throws

Convert a LaunchCodeRequirement to an OnDiskCodeRequirement if possible.

init(ProcessCodeRequirement) throws

Convert a ProcessCodeRequirement to an OnDiskCodeRequirement if possible.

init(from: any Decoder) throws

Create a new instance by decoding from the given decoder

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder

### Type Methods

static func allOf(requirement: () -> [any OnDiskConstraint]) throws -> OnDiskCodeRequirement

Create a OnDiskCodeRequirement that requires matching all of the provided constraints.

static func anyOf(requirement: () -> [any OnDiskConstraint]) throws -> OnDiskCodeRequirement

Create a OnDiskCodeRequirement that requires matching any of the provided constraints.

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

### Checking code requirements for code files on disk

func SecStaticCodeCheckValidityWithOnDiskRequirement(code: SecStaticCode, flags: SecCSFlags, requirement: OnDiskCodeRequirement) -> ValidationResult

Checks whether static code on disk satisfies a lightweight code requirement.

func SecCodeCheckValidityWithOnDiskRequirement(code: SecCode, flags: SecCSFlags, requirement: OnDiskCodeRequirement) -> ValidationResult

Checks whether code on disk satisfies a lightweight code requirement.

struct ValidationResult

A structure that represents the result of testing a lightweight code requirement.

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

