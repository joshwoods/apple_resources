

- Core Media
- CMSimpleQueue
-  CMSimpleQueue.Error 

Structure

# CMSimpleQueue.Error

A structure that defines errors that queue operations can produce.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Error
```

## Topics

### Errors

static let allocationFailed: NSError

The system failed to allocate memory.

static let queueIsFull: NSError

An operation failed because the queue is full.

static let parameterOutOfRange: NSError

You passed a parameter to a function that’s outside the range of allowed values.

static let requiredParameterMissing: NSError

You failed to pass a required parameter to a function.

## Relationships

### Conforms To

- Sendable

