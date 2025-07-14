

- Swift Testing
-  Known issues 

API Collection

# Known issues

Highlight known issues when running tests.

## Overview

The testing library provides a function, `withKnownIssue()`, that you use to mark issues as known. Use this function to inform the testing library at runtime not to mark the test as failing when issues occur.

## Topics

### Recording known issues in tests

func withKnownIssue(Comment?, isIntermittent: Bool, sourceLocation: SourceLocation, () throws -> Void)

Invoke a function that has a known issue that is expected to occur during its execution.

func withKnownIssue(Comment?, isIntermittent: Bool, isolation: isolated (any Actor)?, sourceLocation: SourceLocation, () async throws -> Void) async

Invoke a function that has a known issue that is expected to occur during its execution.

func withKnownIssue(Comment?, isIntermittent: Bool, sourceLocation: SourceLocation, () throws -> Void, when: () -> Bool, matching: KnownIssueMatcher) rethrows

Invoke a function that has a known issue that is expected to occur during its execution.

func withKnownIssue(Comment?, isIntermittent: Bool, isolation: isolated (any Actor)?, sourceLocation: SourceLocation, () async throws -> Void, when: () async -> Bool, matching: KnownIssueMatcher) async rethrows

Invoke a function that has a known issue that is expected to occur during its execution.

typealias KnownIssueMatcher

A function that is used to match known issues.

### Describing a failure or warning

struct Issue

A type describing a failure or warning which occurred during a test.

## See Also

### Behavior validation

Expectations and confirmations

Check for expected values, outcomes, and asynchronous events in tests.

