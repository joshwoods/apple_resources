

- SwiftData
- ModelActor
-  unownedExecutor 

Instance Property

# unownedExecutor

The optimized, unonwned reference to the model actor’s executor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
nonisolated
var unownedExecutor: UnownedSerialExecutor { get }
```

## See Also

### Accessing the executors

var modelExecutor: any ModelExecutor

The executor that coordinates access to the model actor.

**Required**

