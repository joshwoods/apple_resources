

- Swift
-  SerialExecutor 

Protocol

# SerialExecutor

A service that executes jobs.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol SerialExecutor : Executor
```

### Custom Actor Executors

By default, all actor types execute tasks on a shared global concurrent pool. The global pool does not guarantee any thread (or dispatch queue) affinity, so actors are free to use different threads as they execute tasks.

Note

The runtime may perform various optimizations to minimize un-necessary thread switching.

Sometimes it is important to be able to customize the execution behavior of an actor. For example, when an actor is known to perform heavy blocking operations (such as IO), and we would like to keep this work *off* the global shared pool, as blocking it may prevent other actors from being responsive.

You can implement a custom executor, by conforming a type to the SerialExecutor protocol, and implementing the `enqueue(_:)` method.

Once implemented, you can configure an actor to use such executor by implementing the actor’s unownedExecutor computed property. For example, you could accept an executor in the actor’s initializer, store it as a variable (in order to retain it for the duration of the actor’s lifetime), and return it from the `unownedExecutor` computed property like this:

```
actor MyActor {
  let myExecutor: MyExecutor

  // accepts an executor to run this actor on.
  init(executor: MyExecutor) {
    self.myExecutor = executor
  }

  nonisolated var unownedExecutor: UnownedSerialExecutor {
    self.myExecutor.asUnownedSerialExecutor()
  }
}
```

It is also possible to use a form of shared executor, either created as a global or static property, which you can then re-use for every MyActor instance:

```
actor MyActor {
  // Serial executor reused by *all* instances of MyActor!
  static let sharedMyActorsExecutor = MyExecutor() // implements SerialExecutor

  nonisolated var unownedExecutor: UnownedSerialExecutor {
    Self.sharedMyActorsExecutor.asUnownedSerialExecutor()
  }
}
```

In the example above, *all* “MyActor” instances would be using the same serial executor, which would result in only one of such actors ever being run at the same time. This may be useful if some of your code has some “specific thread” requirement when interoperating with non-Swift runtimes for example.

Since the UnownedSerialExecutor returned by the `unownedExecutor` property *does not* retain the executor, you must make sure the lifetime of it extends beyond the lifetime of any actor or task using it, as otherwise it may attempt to enqueue work on a released executor object, causing a crash. The executor returned by unownedExecutor *must* always be the same object, and returning different executors can lead to unexpected behavior.

Alternatively, you can also use existing serial executor implementations, such as Dispatch’s `DispatchSerialQueue` or others.

## Topics

### Instance Methods

func asUnownedSerialExecutor() -> UnownedSerialExecutor

Convert this executor value to the optimized form of borrowed executor references.

**Required** Default implementation provided.

func assertIsolated(@autoclosure () -> String, file: StaticString, line: UInt)

Stops program execution if the current task is not executing on this serial executor.

func checkIsolated()

Last resort “fallback” isolation check, called when the concurrency runtime is comparing executors e.g. during `assumeIsolated()` and is unable to prove serial equivalence between the expected (this object), and the current executor.

**Required** Default implementation provided.

func enqueue(UnownedJob)

**Required**

Deprecated

func enqueue(consuming Job)

**Required**

Deprecated

func enqueue(consuming ExecutorJob)

**Required**

func isSameExclusiveExecutionContext(other: Self) -> Bool

If this executor has complex equality semantics, and the runtime needs to compare two executors, it will first attempt the usual pointer-based equality / check, / and if it fails it will compare the types of both executors, if they are the same, / it will finally invoke this method, in an attempt to let the executor itself decide / if this and the `other` executor represent the same serial, exclusive, isolation context.

**Required** Default implementation provided.

func preconditionIsolated(@autoclosure () -> String, file: StaticString, line: UInt)

Stops program execution if the current task is not executing on this serial executor.

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

