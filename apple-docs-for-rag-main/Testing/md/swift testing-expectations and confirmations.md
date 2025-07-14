

- Swift Testing
-  Expectations and confirmations 

API Collection

# Expectations and confirmations

Check for expected values, outcomes, and asynchronous events in tests.

## Overview

Use expect(_:_:sourceLocation:) and require(_:_:sourceLocation:) macros to validate expected outcomes. To validate that an error is thrown, or *not* thrown, the testing library provides several overloads of the macros that you can use. For more information, see Testing for errors in Swift code.

Use a Confirmation to confirm the occurrence of an asynchronous event that you can’t check directly using an expectation. For more information, see Testing asynchronous code.

### Validate your code’s result

To validate that your code produces an expected value, use expect(_:_:sourceLocation:). This macro captures the expression you pass, and provides detailed information when the code doesn’t satisfy the expectation.

```
@Test func calculatingOrderTotal() {
  let calculator = OrderCalculator()
  #expect(calculator.total(of: [3, 3]) == 7)
  // Prints "Expectation failed: (calculator.total(of: [3, 3]) → 6) == 7"
}
```

Your test keeps running after expect(_:_:sourceLocation:) fails. To stop the test when the code doesn’t satisfy a requirement, use require(_:_:sourceLocation:) instead:

```
@Test func returningCustomerRemembersUsualOrder() throws {
  let customer = try #require(Customer(id: 123))
  // The test runner doesn't reach this line if the customer is nil.
  #expect(customer.usualOrder.countOfItems == 2)
}
```

require(_:_:sourceLocation:) throws an instance of ExpectationFailedError when your code fails to satisfy the requirement.

## Topics

### Checking expectations

macro expect(Bool, @autoclosure () -> Comment?, sourceLocation: SourceLocation)

Check that an expectation has passed after a condition has been evaluated.

macro require(Bool, @autoclosure () -> Comment?, sourceLocation: SourceLocation)

Check that an expectation has passed after a condition has been evaluated and throw an error if it failed.

macro require&lt;T>(T?, @autoclosure () -> Comment?, sourceLocation: SourceLocation) -> T

Unwrap an optional value or, if it is `nil`, fail and throw an error.

### Checking that errors are thrown

Testing for errors in Swift code

Ensure that your code handles errors in the way you expect.

macro expect&lt;E, R>(throws: E.Type, @autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R) -> E?

Check that an expression always throws an error of a given type.

macro expect&lt;E, R>(throws: E, @autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R) -> E?

Check that an expression always throws a specific error.

macro expect&lt;R>(@autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R, throws: (any Error) async throws -> Bool) -> (any Error)?

Check that an expression always throws an error matching some condition.

Deprecated

macro require&lt;E, R>(throws: E.Type, @autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R) -> E

Check that an expression always throws an error of a given type, and throw an error if it does not.

macro require&lt;E, R>(throws: E, @autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R) -> E

macro require&lt;R>(@autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R, throws: (any Error) async throws -> Bool) -> any Error

Check that an expression always throws an error matching some condition, and throw an error if it does not.

Deprecated

### Confirming that asynchronous events occur

Testing asynchronous code

Validate whether your code causes expected events to happen.

func confirmation&lt;R>(Comment?, expectedCount: Int, isolation: isolated (any Actor)?, sourceLocation: SourceLocation, (Confirmation) async throws -> sending R) async rethrows -> R

Confirm that some event occurs during the invocation of a function.

func confirmation&lt;R>(Comment?, expectedCount: some RangeExpression&lt;Int> &amp; Sendable &amp; Sequence&lt;Int>, isolation: isolated (any Actor)?, sourceLocation: SourceLocation, (Confirmation) async throws -> sending R) async rethrows -> R

Confirm that some event occurs during the invocation of a function.

struct Confirmation

A type that can be used to confirm that an event occurs zero or more times.

### Retrieving information about checked expectations

struct Expectation

A type describing an expectation that has been evaluated.

struct ExpectationFailedError

A type describing an error thrown when an expectation fails during evaluation.

protocol CustomTestStringConvertible

A protocol describing types with a custom string representation when presented as part of a test’s output.

### Representing source locations

struct SourceLocation

A type representing a location in source code.

## See Also

### Behavior validation

Known issues

Highlight known issues when running tests.

