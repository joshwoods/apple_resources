

- Swift Testing
-  TestScoping 

Protocol

# TestScoping

A protocol that allows providing a custom execution scope for a test function (and each of its cases) or a test suite by performing custom code before or after it runs.

Swift 6.1+Xcode 16.3+

``` source
protocol TestScoping : Sendable
```

## Overview

Types conforming to this protocol may be used in conjunction with a Trait-conforming type by implementing the scopeProvider(for:testCase:) method, allowing custom traits to provide custom scope for tests. Consolidating common set-up and tear-down logic for tests which have similar needs allows each test function to be more succinct with less repetitive boilerplate so it can focus on what makes it unique.

## Topics

### Instance Methods

func provideScope(for: Test, testCase: Test.Case?, performing: () async throws -> Void) async throws

Provide custom execution scope for a function call which is related to the specified test and/or test case.

**Required**

## Relationships

### Inherits From

- Sendable

## See Also

### Creating custom traits

protocol Trait

A protocol describing traits that can be added to a test function or to a test suite.

protocol TestTrait

A protocol describing traits that can be added to a test function.

protocol SuiteTrait

A protocol describing traits that can be added to a test suite.

