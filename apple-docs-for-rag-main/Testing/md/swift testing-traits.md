

- Swift Testing
-  Traits 

API Collection

# Traits

Add traits to tests to annotate them or customize their behavior.

## Overview

Pass built-in traits to test functions or suite types to comment, categorize, classify, and modify runtime behaviors. You can also use the Trait, TestTrait, and SuiteTrait protocols to create your own types that customize the behavior of test functions.

## Topics

### Customizing runtime behaviors

Enabling and disabling tests

Conditionally enable or disable individual tests before they run.

Limiting the running time of tests

Set limits on how long a test can run for until it fails.

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

static func timeLimit(TimeLimitTrait.Duration) -> Self

Construct a time limit trait that causes a test to time out if it runs for too long.

### Running tests serially or in parallel

Running tests serially or in parallel

Control whether tests run serially or in parallel.

static var serialized: ParallelizationTrait

A trait that serializes the test to which it is applied.

### Annotating tests

Adding tags to tests

Use tags to provide semantic information for organization, filtering, and customizing appearances.

Adding comments to tests

Add comments to provide useful information about tests.

Associating bugs with tests

Associate bugs uncovered or verified by tests.

Interpreting bug identifiers

Examine how the testing library interprets bug identifiers provided by developers.

macro Tag()

Declare a tag that can be applied to a test function or test suite.

static func bug(String, Comment?) -> Self

Construct a bug to track with a test.

static func bug(String?, id: String, Comment?) -> Self

Construct a bug to track with a test.

static func bug(String?, id: some Numeric, Comment?) -> Self

Construct a bug to track with a test.

### Creating custom traits

protocol Trait

A protocol describing traits that can be added to a test function or to a test suite.

protocol TestTrait

A protocol describing traits that can be added to a test function.

protocol SuiteTrait

A protocol describing traits that can be added to a test suite.

protocol TestScoping

A protocol that allows providing a custom execution scope for a test function (and each of its cases) or a test suite by performing custom code before or after it runs.

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

struct TimeLimitTrait

A type that defines a time limit to apply to a test.

