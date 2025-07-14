

- Dispatch
- DispatchQueue
-  concurrentPerform(iterations:execute:) 

Type Method

# concurrentPerform(iterations:execute:)

Submits a single block to the dispatch queue and causes the block to be executed the specified number of times.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
@preconcurrency
class func concurrentPerform(
    iterations: Int,
    execute work: (Int) -> Void
)
```

## Parameters 

`iterations`  

The number of times to execute the block. Higher iteration values give the system the ability to balance more efficiently across multiple cores. To get the maximum benefit of this function, configure the number of iterations to be at least three times the number of available cores.

`work`  

The block to execute in parallel. This block has no return value and takes the following parameter:

iteration  
The current iteration index.

## Discussion

This method implements an efficient parallel for-loop. The dispatch queue executes the submitted block the specified number of times and waits for all iterations to complete before returning. If the target queue is a concurrent queue, the blocks run in parallel and must therefore be reentrant-safe.

