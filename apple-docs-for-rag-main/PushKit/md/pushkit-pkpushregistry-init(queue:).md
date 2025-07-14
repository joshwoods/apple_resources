

- PushKit
- PKPushRegistry
-  init(queue:) 

Initializer

# init(queue:)

Creates a push registry with the specified dispatch queue.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
init(queue: dispatch_queue_t?)
```

## Parameters 

`queue`  

The dispatch queue on which to execute the delegate methods. It is recommended that you specify a serial queue for this parameter. Specify `nil` to execute the delegate methods on the app’s main queue.

## Return Value

A `PKPushRegistry` object that you can use to register for push tokens and use to receive notifications.

