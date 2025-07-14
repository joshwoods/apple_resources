

- Swift Testing
-  ParallelizationTrait 

Structure

# ParallelizationTrait

A type that affects whether or not a test or suite is parallelized.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
struct ParallelizationTrait
```

## Overview

When added to a parameterized test function, this trait causes that test to run its cases serially instead of in parallel. When applied to a non-parameterized test function, this trait has no effect. When applied to a test suite, this trait causes that suite to run its contained test functions and sub-suites serially instead of in parallel.

This trait is recursively applied: if it is applied to a suite, any parameterized tests or test suites contained in that suite are also serialized (as are any tests contained in those suites, and so on.)

This trait does not affect the execution of a test relative to its peers or to unrelated tests. This trait has no effect if test parallelization is globally disabled (by, for example, passing `--no-parallel` to the `swift test` command.)

To add this trait to a test, use serialized.

## Topics

### Instance Properties

var isRecursive: Bool

Whether this instance should be applied recursively to child test suites and test functions or should only be applied to the test suite to which it was directly added.

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

struct Tag

A type representing a tag that can be applied to a test.

struct List

A type representing one or more tags applied to a test.

struct TimeLimitTrait

A type that defines a time limit to apply to a test.

