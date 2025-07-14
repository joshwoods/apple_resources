

- FSKit
- FSUnaryFileSystemOperations
-  probeResource(resource:replyHandler:) 

Instance Method

# probeResource(resource:replyHandler:)

Requests that the file system probe the specified resource.

macOS 15.4+

``` source
func probeResource(
    resource: FSResource,
    replyHandler: @escaping (FSProbeResult?, (any Error)?) -> Void
)
```

**Required**

## Parameters 

`resource`  

The FSResource to probe.

`replyHandler`  

A block or closure that your implementation invokes when it finishes the probe or encounters an error. Pass an instance of FSProbeResult with probe results as the first parameter if your probe operation succeeds. If probing fails, pass an error as the second parameter.

## Discussion

Implement this method to indicate whether the resource is recognizable and usable.

## See Also

### Probing resources

class FSProbeResult

An object that represents the results of a specific probe.

