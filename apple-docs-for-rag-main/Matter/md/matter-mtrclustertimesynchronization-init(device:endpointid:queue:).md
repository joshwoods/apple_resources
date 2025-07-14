

- Matter
- MTRClusterTimeSynchronization
-  init(device:endpointID:queue:) 

Initializer

# init(device:endpointID:queue:)

For all instance methods that take a completion (i.e. command invocations), the completion will be called on the provided queue.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
init?(
    device: MTRDevice,
    endpointID: NSNumber,
    queue: dispatch_queue_t
)
```

