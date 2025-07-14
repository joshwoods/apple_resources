

- os
- OSSignposter
-  withIntervalSignpost(\_:id:around:) 

Instance Method

# withIntervalSignpost(\_:id:around:)

Measures the execution of the specified closure.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func withIntervalSignpost(
    _ name: StaticString,
    id: OSSignpostID = .exclusive,
    around task: () throws -> T
) rethrows -> T
```

## Parameters 

`name`  

The signpost’s name.

`id`  

The signpost’s ID. The default value is exclusive.

`task`  

The closure around which to create the signposted interval.

## Discussion

The signposter uses a signpost ID to pair the beginning and the end of a signposted interval, which is necessary because multiple intervals with the same configuration and scope can be in-flight simultaneously. If only one interval with a specific configuration can execute at any particular time, pass exclusive as the `id` parameter. Otherwise, use the makeSignpostID() and makeSignpostID(from:) methods to generate a signpost identifier, as the following example shows:

```
// Create a signposter using the default subsystem.
let signposter = OSSignposter()

// Generate a signpost ID to associate with the signpost.
let signpostID = signposter.makeSignpostID()

// Signpost the interval of a closure that encapsulates 
// one or more related tasks.
signposter.withIntervalSignpost("Example Signpost", id: signpostID) {
    // Perform one or more related tasks.
}
```

## See Also

### Measuring a Closure

func withIntervalSignpost&lt;T>(StaticString, id: OSSignpostID, SignpostMetadata, around: () throws -> T) rethrows -> T

Measures the execution of a closure and attaches the specified message.

