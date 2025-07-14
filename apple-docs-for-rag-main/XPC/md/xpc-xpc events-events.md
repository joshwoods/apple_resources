

- XPC
-  XPC events 

API Collection

# XPC events

Respond on demand to IOKit events and notifications.

## Topics

### Event handling

func xpc_set_event_stream_handler(UnsafePointer&lt;CChar>, dispatch_queue_t?, xpc_handler_t)

Sets the event handler to invoke when receiving streamed events.

let XPC_EVENT_KEY_NAME: UnsafePointer&lt;CChar>

A key for querying an XPC event dictionary to retrieve a string that identifies the event.

