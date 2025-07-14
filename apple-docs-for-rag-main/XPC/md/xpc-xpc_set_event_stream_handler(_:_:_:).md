

- XPC
-  xpc_set_event_stream_handler(\_:\_:\_:) 

Function

# xpc_set_event_stream_handler(\_:\_:\_:)

Sets the event handler to invoke when receiving streamed events.

macOS 10.7+

``` source
func xpc_set_event_stream_handler(
    _ stream: UnsafePointer,
    _ targetq: dispatch_queue_t?,
    _ handler: @escaping xpc_handler_t
)
```

## Parameters 

`stream`  

The name of the event stream for which this handler will be invoked.

`targetq`  

The GCD queue to which the event handler block will be submitted. This parameter may be NULL, in which case the connection’s target queue will be the default target queue of `libdispatch`, defined as `DISPATCH_TARGET_QUEUE_DEFAULT`.

`handler`  

The event handler block. The event which this block receives as its first parameter will always be a dictionary which contains the XPC_EVENT_KEY_NAME key. The value for this key will be a string whose value is the name assigned to the XPC event specified in the `launchd.plist`. Future keys may be added to this dictionary.

## Discussion

Multiple calls to this function for the same event stream will result in undefined behavior.

## See Also

### Event handling

let XPC_EVENT_KEY_NAME: UnsafePointer&lt;CChar>

A key for querying an XPC event dictionary to retrieve a string that identifies the event.

