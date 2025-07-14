

- Swift
-  UnownedTaskExecutor 

Structure

# UnownedTaskExecutor

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@frozen
struct UnownedTaskExecutor
```

## Topics

### Initializers

init(Builtin.Executor)

init&lt;E>(ordinary: E)

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
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

struct UnownedSerialExecutor

An unowned reference to a serial executor (a `SerialExecutor` value).

var globalConcurrentExecutor: any TaskExecutor

The global concurrent executor that is used by default for Swift Concurrency tasks.

func withTaskExecutorPreference&lt;T, Failure>((any TaskExecutor)?, isolation: isolated (any Actor)?, operation: () async throws(Failure) -> T) async throws(Failure) -> T

Configure the current task hierarchy’s task executor preference to the passed TaskExecutor, and execute the passed in closure by immediately hopping to that executor.

