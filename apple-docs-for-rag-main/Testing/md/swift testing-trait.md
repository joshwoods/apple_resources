

- Swift Testing
-  Trait 

Protocol

# Trait

A protocol describing traits that can be added to a test function or to a test suite.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
protocol Trait : Sendable
```

## Overview

The testing library defines a number of traits that can be added to test functions and to test suites. Developers can define their own traits by creating types that conform to TestTrait and/or SuiteTrait.

When creating a custom trait type, the type should conform to TestTrait if it can be added to test functions, SuiteTrait if it can be added to test suites, and both TestTrait and SuiteTrait if it can be added to both test functions *and* test suites.

## Topics

### Enabling and disabling tests

static func enabled(if: @autoclosure () throws -> Bool, Comment?, sourceLocation: SourceLocation) -> Self

Construct a condition trait that causes a test to be disabled if it returns `false`.

static func enabled(Comment?, sourceLocation: SourceLocation, () async throws -> Bool) -> Self

Construct a condition trait that causes a test to be disabled if it returns `false`.

static func disabled(Comment?, sourceLocation: SourceLocation) -> Self

Construct a condition trait that disables a test unconditionally.

static func disabled(if: @autoclosure () throws -> Bool, Comment?, sourceLocation: SourceLocation) -> Self

Construct a condition trait that causes a test to be disabled if it returns `true`.

static func disabled(Comment?, sourceLocation: SourceLocation, () async throws -> Bool) -> Self

Construct a condition trait that causes a test to be disabled if it returns `true`.

### Limiting the running time of tests

static func timeLimit(TimeLimitTrait.Duration) -> Self

Construct a time limit trait that causes a test to time out if it runs for too long.

### Running tests serially or in parallel

static var serialized: ParallelizationTrait

A trait that serializes the test to which it is applied.

### Categorizing tests

static func tags(Tag...) -> Self

Construct a list of tags to apply to a test.

### Associating bugs

static func bug(String, Comment?) -> Self

Construct a bug to track with a test.

static func bug(String?, id: String, Comment?) -> Self

Construct a bug to track with a test.

static func bug(String?, id: some Numeric, Comment?) -> Self

Construct a bug to track with a test.

### Adding information to tests

var comments: [Comment]

The user-provided comments for this trait, if any.

**Required** Default implementation provided.

### Preparing internal state

func prepare(for: Test) async throws

Prepare to run the test to which this trait was added.

**Required** Default implementation provided.

### Providing custom execution scope for tests

protocol TestScoping

A protocol that allows providing a custom execution scope for a test function (and each of its cases) or a test suite by performing custom code before or after it runs.

func scopeProvider(for: Test, testCase: Test.Case?) -> Self.TestScopeProvider?

Get this trait’s scope provider for the specified test and/or test case, if any.

**Required** Default implementations provided.

associatedtype TestScopeProvider : TestScoping = Never

The type of the test scope provider for this trait.

**Required**

## Relationships

### Inherits From

- Sendable

### Inherited By

- SuiteTrait
- TestTrait

### Conforming Types

- Bug
- Comment
- ConditionTrait
- ParallelizationTrait
- Tag.List
- TimeLimitTrait

## See Also

### Creating custom traits

protocol TestTrait

A protocol describing traits that can be added to a test function.

protocol SuiteTrait

A protocol describing traits that can be added to a test suite.

protocol TestScoping

A protocol that allows providing a custom execution scope for a test function (and each of its cases) or a test suite by performing custom code before or after it runs.

