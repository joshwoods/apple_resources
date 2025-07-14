

- Swift
- UnownedJob
-  runSynchronously(on:) 

Instance Method

# runSynchronously(on:)

Run this job on the passed in executor.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func runSynchronously(on executor: UnownedSerialExecutor)
```

## Parameters 

`executor`  

The executor this job will be semantically running on.

## Discussion

This operation runs the job on the calling thread and *blocks* until the job completes. The intended use of this method is for an executor to determine when and where it wants to run the job and then call this method on it.

The passed in executor reference is used to establish the executor context for the job, and should be the same executor as the one semantically calling the `runSynchronously` method.

