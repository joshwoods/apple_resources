

- CallKit
- CXCallController
-  init(queue:) 

Initializer

# init(queue:)

Initializes a new call controller with a specified queue, which is used for calling completion blocks.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
init(queue: dispatch_queue_t)
```

## Parameters 

`queue`  

The queue used for calling completion blocks.

## Return Value

A new call controller initialized with the specified queue.

## Discussion

This is the designated initializer.

## See Also

### Creating New Call Controllers

convenience init()

Initializes a new call controller with a private, serial queue, which is used for calling completion blocks.

