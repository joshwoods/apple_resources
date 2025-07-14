

- Swift
-  ExecutorJob 

Structure

# ExecutorJob

A unit of schedulable work.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@frozen
struct ExecutorJob
```

## Overview

Unless you’re implementing a scheduler, you don’t generally interact with jobs directly.

## Topics

### Initializers

init(Job)

init(UnownedJob)

### Instance Properties

var description: String

var priority: JobPriority

### Instance Methods

func runSynchronously(isolatedTo: UnownedSerialExecutor, taskExecutor: UnownedTaskExecutor)

Run this job isolated to the passed in serial executor, while executing it on the specified task executor.

func runSynchronously(on: UnownedTaskExecutor)

Run this job on the passed in task executor.

func runSynchronously(on: UnownedSerialExecutor)

Run this job on the passed in executor.

## Relationships

### Conforms To

- Sendable

## See Also

### Executors

protocol Executor

A service that can execute jobs.

protocol SerialExecutor

A service that executes jobs.

protocol TaskExecutor

An executor that may be used as preferred executor by a task.

typealias PartialAsyncTaskDeprecated

struct UnownedJob

A unit of schedulable work.

struct JobPriority

The priority of this job.

struct UnownedSerialExecutor

An unowned reference to a serial executor (a `SerialExecutor` value).

struct UnownedTaskExecutor

var globalConcurrentExecutor: any TaskExecutor

The global concurrent executor that is used by default for Swift Concurrency tasks.

func withTaskExecutorPreference&lt;T, Failure>((any TaskExecutor)?, isolation: isolated (any Actor)?, operation: () async throws(Failure) -> T) async throws(Failure) -> T

Configure the current task hierarchy’s task executor preference to the passed TaskExecutor, and execute the passed in closure by immediately hopping to that executor.

