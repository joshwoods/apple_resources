

- Swift
-  CancellationError 

Structure

# CancellationError

An error that indicates a task was canceled.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct CancellationError
```

## Overview

This error is also thrown automatically by `Task.checkCancellation()`, if the current task has been canceled.

## Topics

### Initializers

init()

## Relationships

### Conforms To

- Error
- Sendable

## See Also

### Canceling Tasks

func cancel()

Cancels this task.

var isCancelled: Bool

A Boolean value that indicates whether the task should stop executing.

static var isCancelled: Bool

A Boolean value that indicates whether the task should stop executing.

static func checkCancellation() throws

Throws an error if the task was canceled.

func withTaskCancellationHandler&lt;T>(handler: () -> Void, operation: () async throws -> T) async rethrows -> TDeprecated

