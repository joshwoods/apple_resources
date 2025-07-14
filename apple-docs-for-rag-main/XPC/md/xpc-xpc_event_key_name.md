

- XPC
-  XPC_EVENT_KEY_NAME 

Global Variable

# XPC_EVENT_KEY_NAME

A key for querying an XPC event dictionary to retrieve a string that identifies the event.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOS 9.0+watchOS 2.0+

``` source
let XPC_EVENT_KEY_NAME: UnsafePointer
```

## See Also

### Event handling

func xpc_set_event_stream_handler(UnsafePointer&lt;CChar>, dispatch_queue_t?, xpc_handler_t)

Sets the event handler to invoke when receiving streamed events.

