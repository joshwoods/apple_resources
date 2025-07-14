

- Swift
-  globalConcurrentExecutor 

Global Variable

# globalConcurrentExecutor

The global concurrent executor that is used by default for Swift Concurrency tasks.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var globalConcurrentExecutor: any TaskExecutor { get }
```

## Discussion

The executor’s implementation is platform dependent. By default it uses a fixed size pool of threads and should not be used for blocking operations which do not guarantee forward progress as doing so may prevent other tasks from being executed and render the system unresponsive.

You may pass this executor explicitly to a Task initializer as a task executor preference, in order to ensure and document that task be executed on the global executor, instead e.g. inheriting the enclosing actor’s executor. Refer to `withTaskExecutorPreference(_:operation:)` for a detailed discussion of task executor preferences.

Customizing the global concurrent executor is currently not supported.

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

struct UnownedTaskExecutor

func withTaskExecutorPreference&lt;T, Failure>((any TaskExecutor)?, isolation: isolated (any Actor)?, operation: () async throws(Failure) -> T) async throws(Failure) -> T

Configure the current task hierarchy’s task executor preference to the passed TaskExecutor, and execute the passed in closure by immediately hopping to that executor.

