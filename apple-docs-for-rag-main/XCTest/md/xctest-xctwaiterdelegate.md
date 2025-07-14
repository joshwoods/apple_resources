

- XCTest
-  XCTWaiterDelegate 

Protocol

# XCTWaiterDelegate

Defines methods that are called when XCTWaiter expectations are fulfilled correctly or incorrectly.

``` source
protocol XCTWaiterDelegate : NSObjectProtocol
```

## Overview

XCTestCase instances automatically conform to the XCTWaiterDelegate protocol. If you pass a test case instance as the delegate property of XCTWaiter’s init(delegate:) initializer, that test case will automatically report timeouts and other unexpected events as test failures.

## Topics

### Timeout Events

func waiter(XCTWaiter, didTimeoutWithUnfulfilledExpectations: [XCTestExpectation])

Invoked when not all waited on expectations are fulfilled during the timeout period.

func nestedWaiter(XCTWaiter, wasInterruptedByTimedOutWaiter: XCTWaiter)

Invoked when the waiter is interrupted prior to its expectations being fulfilled or timing out.

### Order of Fulfillment Events

func waiter(XCTWaiter, fulfillmentDidViolateOrderingConstraintsFor: XCTestExpectation, requiredExpectation: XCTestExpectation)

Invoked when a waiter is enforcing fulfillment order and an expectation is fulfilled in the wrong order.

### Inverted Expectation Events

func waiter(XCTWaiter, didFulfillInvertedExpectation: XCTestExpectation)

Invoked when an expectation whose `isInverted` property is set to `true` is fulfilled.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- XCTestCase

## See Also

### Responding to Expectation Fulfilment

var delegate: (any XCTWaiterDelegate)?

The delegate to which expectation fulfillment events will be reported.

var fulfilledExpectations: [XCTestExpectation]

An array of expectations that were fulfilled, in order, up until the waiter stopped waiting.

