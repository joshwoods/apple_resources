

- SwiftData
- ModelActor
-  modelExecutor 

Instance Property

# modelExecutor

The executor that coordinates access to the model actor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
nonisolated
var modelExecutor: any ModelExecutor { get }
```

**Required**

## Discussion

Important

Don’t use the executor to access the model context. Instead, use the modelContext property.

## See Also

### Accessing the executors

var unownedExecutor: UnownedSerialExecutor

The optimized, unonwned reference to the model actor’s executor.

