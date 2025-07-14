

- XCTest
-  Asynchronous Tests and Expectations 

API Collection

# Asynchronous Tests and Expectations

Verify that asynchronous code behaves as expected.

## Overview

Asynchronous code doesn’t execute directly within the current flow of code. This might be because the code runs on a different thread or dispatch queue, in a delegate method, or in a callback, or because it’s a Swift function marked with `async`.

`XCTest` provides two approaches for testing asynchronous code. For Swift code that uses `async` and `await` for concurrency, you mark your test methods `async` or `async` `throws` to test asynchronously. For any other types of asynchronous code, within your test you create one or more *expectations*, which are objects that XCTest uses to handle waiting. Then you *fulfill* those expectations when the asynchronous code finishes running to tell XCTest to stop waiting. Your test method waits until all expectations are fulfilled or a specified timeout expires.

### Build Asynchronous Tests with Swift Concurrency

To test Swift code that uses `async` and `await` for concurrency, mark your test method `async` or `async` `throws`. `XCTest` executes your test method asynchronously so that your test waits until `async` calls complete.

```
```

When the asynchronous task completes, perform assertions to confirm that the task’s actual results meet your expected results.

If your test encounters a thrown error, `XCTest` records a test failure.

Important

If your test code needs to run on the Main actor, specify `@MainActor` for your test method or class. If you don’t specify an actor, the test method executes on an arbitrary actor.

### Build Asynchronous Tests with Expectations

When you can’t use Swift `async`, use expectations to test asynchronous code. For example, use expectations when there isn’t a Swift `async` alternative available or when your asynchronous code runs in:

- Objective-C

- An asynchronous block in a dispatch queue

- A delegate method

- An asynchronous callback, closure, or completion block

- A `Future` or `Promise` in Swift Combine

- A situation where it needs to complete within a specific amount of time

Before you perform an asynchronous task in your test method, create an instance of XCTestExpectation with a description of the task.

```
```

Start the asynchronous task, and then tell the test to wait for the expectation to complete within an amount of time you specify.

```
```

When the asynchronous task returns (for example, in a callback), perform assertions to confirm that the task’s actual results meet your expected results. When the task completes, call the fulfill() method on the expectation to indicate to the test that it can stop waiting and proceed with the next test.

```
```

If the test doesn’t execute the `fulfill()` method before the wait statement’s timeout expires, `XCTest` records a test failure.

## Topics

### Expectations

class XCTestExpectation

An expected outcome in an asynchronous test.

### Key Value Observing Expectations

class XCTKVOExpectation

An expectation that a specific key-value observing (KVO) condition fulfills.

class XCTKeyPathExpectation

An expectation that a specific key-value observing (KVO) condition fulfills.

### Notification-Based Expectations

class XCTNSNotificationExpectation

An expectation that is fulfilled when an expected `NSNotification` is received.

class XCTDarwinNotificationExpectation

An expectation that is fulfilled when an expected Darwin notification is received.

### Predicate-Based Expectations

class XCTNSPredicateExpectation

An expectation that’s fulfilled when an `NSPredicate` is satisfied.

### Expectation Waiters

class XCTWaiter

Waits for the fulfillment of a group of expectations.

