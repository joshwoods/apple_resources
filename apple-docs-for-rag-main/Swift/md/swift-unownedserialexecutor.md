

- Swift
-  UnownedSerialExecutor 

Structure

# UnownedSerialExecutor

An unowned reference to a serial executor (a `SerialExecutor` value).

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct UnownedSerialExecutor
```

## Overview

This is an optimized type used internally by the core scheduling operations. It is an unowned reference to avoid unnecessary reference-counting work even when working with actors abstractly. Generally there are extra constraints imposed on core operations in order to allow this. For example, keeping an actor alive must also keep the actor’s associated executor alive; if they are different objects, the executor must be referenced strongly by the actor.

## Topics

### Initializers

init(Builtin.Executor)

init&lt;E>(complexEquality: E)

Opts the executor into complex “same exclusive execution context” equality checks.

init&lt;E>(ordinary: E)

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Sendable

## See Also

### Executors

protocol Executor

A service that can execute jobs.

struct ExecutorJob

A unit of schedulable work.

protocol SerialExecutor

A service that executes jobs.

protocol TaskExecutor

An executor that may be used as preferred executor by a task.

typealias PartialAsyncTaskDeprecated

struct UnownedJob

A unit of schedulable work.

struct JobPriority

The priority of this job.

struct UnownedTaskExecutor

var globalConcurrentExecutor: any TaskExecutor

The global concurrent executor that is used by default for Swift Concurrency tasks.

func withTaskExecutorPreference&lt;T, Failure>((any TaskExecutor)?, isolation: isolated (any Actor)?, operation: () async throws(Failure) -> T) async throws(Failure) -> T

Configure the current task hierarchy’s task executor preference to the passed TaskExecutor, and execute the passed in closure by immediately hopping to that executor.

