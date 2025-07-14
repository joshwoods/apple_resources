

- Swift
-  UnownedJob 

Structure

# UnownedJob

A unit of schedulable work.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct UnownedJob
```

## Overview

Unless you’re implementing a scheduler, you don’t generally interact with jobs directly.

An `UnownedJob` must be eventually run *exactly once* using `runSynchronously(on:)`. Not doing so is effectively going to leak and “hang” the work that the job represents (e.g. a Task).

## Topics

### Initializers

init(ExecutorJob)

Create an `UnownedJob` whose lifetime must be managed carefully until it is run exactly once.

init(Job)

Create an `UnownedJob` whose lifetime must be managed carefully until it is run exactly once.

### Instance Properties

var priority: JobPriority

The priority of this job.

### Instance Methods

func runSynchronously(isolatedTo: UnownedSerialExecutor, taskExecutor: UnownedTaskExecutor)

Run this job isolated to the passed in serial executor, while executing it on the specified task executor.

func runSynchronously(on: UnownedTaskExecutor)

Run this job isolated to the passed task executor.

func runSynchronously(on: UnownedSerialExecutor)

Run this job on the passed in executor.

### Default Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- CustomStringConvertible
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

struct JobPriority

The priority of this job.

struct UnownedSerialExecutor

An unowned reference to a serial executor (a `SerialExecutor` value).

struct UnownedTaskExecutor

var globalConcurrentExecutor: any TaskExecutor

The global concurrent executor that is used by default for Swift Concurrency tasks.

func withTaskExecutorPreference&lt;T, Failure>((any TaskExecutor)?, isolation: isolated (any Actor)?, operation: () async throws(Failure) -> T) async throws(Failure) -> T

Configure the current task hierarchy’s task executor preference to the passed TaskExecutor, and execute the passed in closure by immediately hopping to that executor.

