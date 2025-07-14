

- Swift
-  withTaskExecutorPreference(\_:isolation:operation:) 

Function

# withTaskExecutorPreference(\_:isolation:operation:)

Configure the current task hierarchy’s task executor preference to the passed TaskExecutor, and execute the passed in closure by immediately hopping to that executor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func withTaskExecutorPreference(
    _ taskExecutor: (any TaskExecutor)?,
    isolation: isolated (any Actor)? = #isolation,
    operation: () async throws(Failure) -> T
) async throws(Failure) -> T where Failure : Error
```

## Parameters 

`taskExecutor`  

The executor to use as preferred task executor for this operation, and any child tasks created inside the `operation` closure. If `nil` it is interpreted as “no preference” and calling this method will have no impact on execution semantics of the `operation`

`operation`  

The operation to execute on the passed executor

## Return Value

The value returned from the `operation` closure

### Task executor preference semantics

Task executors influence *where* nonisolated asynchronous functions, and default actor methods execute. The preferred executor will be used whenever possible, rather than hopping to the global concurrent pool.

For an in depth discussion of this topic, see TaskExecutor.

### Disabling task executor preference

Passing `nil` as executor means disabling any preference preference (if it was set) and the task hierarchy will execute without any executor preference until a different preference is set.

### Asynchronous function execution semantics in presence of task executor preferences

The following diagram illustrates on which executor an `async` function will execute, in presence (or lack thereof) a task executor preference.

```
[ func / closure ] - /* where should it execute? */
                              |
                    +--------------+          +===========================+
          +-------- | is isolated? | - yes -> | actor has unownedExecutor |
          |         +--------------+          +===========================+
          |                                       |                |
          |                                      yes               no
          |                                       |                |
          |                                       v                v
          |                  +=======================+    /* task executor preference? */
          |                  | on specified executor |        |                   |
          |                  +=======================+       yes                  no
          |                                                   |                   |
          |                                                   |                   v
          |                                                   |    +==========================+
          |                                                   |    | default (actor) executor |
          |                                                   v    +==========================+
          v                                     +==============================+
 /* task executor preference? */ ---- yes ----> | on Task's preferred executor |
          |                                     +==============================+
          no
          |
          v
 +===============================+
 | on global concurrent executor |
 +===============================+
```

In short, without a task executor preference, `nonisolated async` functions will execute on the global concurrent executor. If a task executor preference is present, such `nonisolated async` functions will execute on the preferred task executor.

Isolated functions semantically execute on the actor they are isolated to, however if such actor does not declare a custom executor (it is a “default actor”) in presence of a task executor preference, tasks executing on this actor will use the preferred executor as source of threads to run the task, while isolated on the actor.

### Example

```
Task {
  // case 0) "no task executor preference"

  // default task executor
  // ...
  await SomeDefaultActor().hello() // default executor
  await ActorWithCustomExecutor().hello() // 'hello' executes on actor's custom executor

  // child tasks execute on default executor:
  async let x = ...
  await withTaskGroup(of: Int.self) { group in g.addTask { 7 } }

  await withTaskExecutorPreference(specific) {
    // case 1) 'specific' task executor preference

    // 'specific' task executor
    // ...
    await SomeDefaultActor().hello() // 'hello' executes on 'specific' executor
    await ActorWithCustomExecutor().hello() // 'hello' executes on actor's custom executor (same as case 0)

    // child tasks execute on 'specific' task executor:
    async let x = ...
    await withTaskGroup(of: Int.self) { group in
      group.addTask { 7 } // child task executes on 'specific' executor
      group.addTask(executorPreference: globalConcurrentExecutor) { 13 } // child task executes on global concurrent executor
    }

    // disable the task executor preference:
    await withTaskExecutorPreference(globalConcurrentExecutor) {
      // equivalent to case 0) preference is globalConcurrentExecutor

      // default task executor
      // ...
      await SomeDefaultActor().hello() // default executor (same as case 0)
      await ActorWithCustomExecutor().hello() // 'hello' executes on actor's custom executor (same as case 0)

      // child tasks execute on default executor (same as case 0):
      async let x = ...
      await withTaskGroup(of: Int.self) { group in g.addTask { 7 } }
    }
  }
}
```

Throws

If the operation closure throws

See Also

TaskExecutor

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

var globalConcurrentExecutor: any TaskExecutor

The global concurrent executor that is used by default for Swift Concurrency tasks.

