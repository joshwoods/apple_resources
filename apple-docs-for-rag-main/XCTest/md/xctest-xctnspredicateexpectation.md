

- XCTest
-  XCTNSPredicateExpectation 

Class

# XCTNSPredicateExpectation

An expectation that’s fulfilled when an `NSPredicate` is satisfied.

``` source
class XCTNSPredicateExpectation
```

## Overview

When you use an instance of this class from Swift and await using fulfillment(of:timeout:enforceOrder:) rather than wait(for:), XCTest evaluates the associated predicate on the main actor.

## Topics

### Creating a Predicate-Based Expectation

init(predicate: NSPredicate, object: Any?)

Creates an expectation that’s fulfilled when an `NSPredicate` instance returns `true`, optionally for a provided object.

### Expectation Properties

var predicate: NSPredicate

The predicate the expectation evaluates.

var object: Any?

An optional object against which the predicate evaluates.

### Handling Predicate Resolution

var handler: XCTNSPredicateExpectation.Handler?

An optional handler that performs custom evaluation when `predicate` evaluates as `true`.

typealias Handler

A handler XCTest calls when evaluating the predicate returns `true`.

## Relationships

### Inherits From

- XCTestExpectation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

