

- Swift
- ExecutorJob
-  runSynchronously(on:) 

Instance Method

# runSynchronously(on:)

Run this job on the passed in task executor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func runSynchronously(on executor: UnownedTaskExecutor)
```

## Parameters 

`executor`  

The executor this job will be run on.

## Discussion

This operation runs the job on the calling thread and *blocks* until the job completes. The intended use of this method is for an executor to determine when and where it wants to run the job and then call this method on it.

The passed in executor reference is used to establish the executor context for the job, and should be the same executor as the one semantically calling the `runSynchronously` method.

This operation consumes the job, preventing it accidental use after it has been run.

Converting a `ExecutorJob` to an UnownedJob and invoking \`\`UnownedJob/runSynchronously(\_:)\` on it multiple times is undefined behavior, as a job can only ever be run once, and must not be accessed after it has been run.

See Also

runSynchronously(isolatedTo:taskExecutor:)

