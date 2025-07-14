

- Swift Testing
-  Test 

Structure

# Test

A type representing a test or suite.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
struct Test
```

## Overview

An instance of this type may represent:

- A type containing zero or more tests (i.e. a *test suite*);

- An individual test function (possibly contained within a type); or

- A test function parameterized over one or more sequences of inputs.

Two instances of this type are considered to be equal if the values of their id properties are equal.

## Topics

### Structures

struct Case

A single test case from a parameterized Test.

### Instance Properties

var associatedBugs: [Bug]

The set of bugs associated with this test.

var comments: [Comment]

The complete set of comments about this test from all of its traits.

var displayName: String?

The customized display name of this instance, if specified.

var isParameterized: Bool

Whether or not this test is parameterized.

var isSuite: Bool

Whether or not this instance is a test suite containing other tests.

var name: String

The name of this instance.

var sourceLocation: SourceLocation

The source location of this test.

var tags: Set&lt;Tag>

The complete, unique set of tags associated with this test.

var timeLimit: Duration?

The maximum amount of time the cases of this test may run for.

var traits: [any Trait]

The set of traits added to this instance when it was initialized.

### Type Properties

static var current: Test?

The test that is running on the current task, if any.

### Default Implementations

Equatable Implementations

Hashable Implementations

Identifiable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Identifiable
- Sendable

## See Also

### Essentials

Defining test functions

Define a test function to validate that code is working correctly.

Organizing test functions with suite types

Organize tests into test suites.

Migrating a test from XCTest

Migrate an existing test method or test class written using XCTest.

macro Test(String?, any TestTrait...)

Declare a test.

macro Suite(String?, any SuiteTrait...)

Declare a test suite.

