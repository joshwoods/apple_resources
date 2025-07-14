

- Swift
-  TaskExecutor 

Protocol

# TaskExecutor

An executor that may be used as preferred executor by a task.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol TaskExecutor : Executor
```

### Impact of setting a task executor preference

By default, without setting a task executor preference, nonisolated asynchronous functions, as well as methods declared on default actors – that is actors which do not require a specific executor – execute on Swift’s default global concurrent executor. This is an executor shared by the entire runtime to execute any work which does not have strict executor requirements.

By setting a task executor preference, either with a `withTaskExecutorPreference(_:operation:)`, creating a task with a preference (`Task(executorPreference:)`, or `group.addTask(executorPreference:)`), the task and all of its child tasks (unless a new preference is set) will be preferring to execute on the provided task executor.

Unstructured tasks do not inherit the task executor.

## Topics

### Instance Methods

func asUnownedTaskExecutor() -> UnownedTaskExecutor

**Required** Default implementation provided.

func enqueue(consuming ExecutorJob)

**Required**

func enqueue(consuming Job)

**Required**

Deprecated

func enqueue(UnownedJob)

**Required**

## Relationships

### Inherits From

- Executor
- Sendable

## See Also

### Executors

protocol Executor

A service that can execute jobs.

struct ExecutorJob

A unit of schedulable work.

protocol SerialExecutor

A service that executes jobs.

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

