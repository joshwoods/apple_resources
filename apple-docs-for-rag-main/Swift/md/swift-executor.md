

- Swift
-  Executor 

Protocol

# Executor

A service that can execute jobs.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol Executor : AnyObject, Sendable
```

## Topics

### Instance Methods

func enqueue(consuming Job)

**Required** Default implementations provided.

Deprecated

func enqueue(consuming ExecutorJob)

**Required** Default implementations provided.

func enqueue(UnownedJob)

**Required** Default implementations provided.

## Relationships

### Inherits From

- Sendable

### Inherited By

- SerialExecutor
- TaskExecutor

## See Also

### Executors

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

struct UnownedSerialExecutor

An unowned reference to a serial executor (a `SerialExecutor` value).

struct UnownedTaskExecutor

var globalConcurrentExecutor: any TaskExecutor

The global concurrent executor that is used by default for Swift Concurrency tasks.

func withTaskExecutorPreference&lt;T, Failure>((any TaskExecutor)?, isolation: isolated (any Actor)?, operation: () async throws(Failure) -> T) async throws(Failure) -> T

Configure the current task hierarchy’s task executor preference to the passed TaskExecutor, and execute the passed in closure by immediately hopping to that executor.

