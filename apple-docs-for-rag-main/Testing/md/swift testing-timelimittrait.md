

- Swift Testing
-  TimeLimitTrait 

Structure

# TimeLimitTrait

A type that defines a time limit to apply to a test.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+Swift 6.0+Xcode 16.0+

``` source
struct TimeLimitTrait
```

## Overview

To add this trait to a test, use one of the following functions:

- timeLimit(_:)

## Topics

### Structures

struct Duration

A type representing the duration of a time limit applied to a test.

### Instance Properties

var isRecursive: Bool

Whether this instance should be applied recursively to child test suites and test functions or should only be applied to the test suite to which it was directly added.

var timeLimit: Duration

The maximum amount of time a test may run for before timing out.

### Type Aliases

typealias TestScopeProvider

The type of the test scope provider for this trait.

### Default Implementations

Trait Implementations

## Relationships

### Conforms To

- Sendable
- SuiteTrait
- TestTrait
- Trait

## See Also

### Supporting types

struct Bug

A type representing a bug report tracked by a test.

struct Comment

A type representing a comment related to a test.

struct ConditionTrait

A type that defines a condition which must be satisfied for a test to be enabled.

struct ParallelizationTrait

A type that affects whether or not a test or suite is parallelized.

struct Tag

A type representing a tag that can be applied to a test.

struct List

A type representing one or more tags applied to a test.

