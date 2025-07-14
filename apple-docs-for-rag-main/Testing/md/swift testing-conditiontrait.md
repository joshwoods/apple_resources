

- Swift Testing
-  ConditionTrait 

Structure

# ConditionTrait

A type that defines a condition which must be satisfied for a test to be enabled.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
struct ConditionTrait
```

## Mentioned in 

Migrating a test from XCTest

## Overview

To add this trait to a test, use one of the following functions:

- enabled(if:_:sourceLocation:)

- enabled(_:sourceLocation:_:)

- disabled(_:sourceLocation:)

- disabled(if:_:sourceLocation:)

- disabled(_:sourceLocation:_:)

## Topics

### Instance Properties

var comments: [Comment]

The user-provided comments for this trait, if any.

var isRecursive: Bool

Whether this instance should be applied recursively to child test suites and test functions or should only be applied to the test suite to which it was directly added.

var sourceLocation: SourceLocation

The source location where this trait was specified.

### Instance Methods

func prepare(for: Test) async throws

Prepare to run the test to which this trait was added.

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

struct ParallelizationTrait

A type that affects whether or not a test or suite is parallelized.

struct Tag

A type representing a tag that can be applied to a test.

struct List

A type representing one or more tags applied to a test.

struct TimeLimitTrait

A type that defines a time limit to apply to a test.

