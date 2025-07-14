

- CallKit
- CXCallController
-  init() 

Initializer

# init()

Initializes a new call controller with a private, serial queue, which is used for calling completion blocks.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
convenience init()
```

## Return Value

A new call controller initialized with a private, serial queue.

## See Also

### Creating New Call Controllers

init(queue: dispatch_queue_t)

Initializes a new call controller with a specified queue, which is used for calling completion blocks.

