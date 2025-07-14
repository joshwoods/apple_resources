

- Core Foundation
-  CFMessagePortSendRequest(\_:\_:\_:\_:\_:\_:\_:) 

Function

# CFMessagePortSendRequest(\_:\_:\_:\_:\_:\_:\_:)

Sends a message to a remote CFMessagePort object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFMessagePortSendRequest(
    _ remote: CFMessagePort!,
    _ msgid: Int32,
    _ data: CFData!,
    _ sendTimeout: CFTimeInterval,
    _ rcvTimeout: CFTimeInterval,
    _ replyMode: CFString!,
    _ returnData: UnsafeMutablePointer?>!
) -> Int32
```

## Parameters 

`remote`  

The message port to which `data` should be sent.

`msgid`  

An arbitrary integer value that you can send with the message.

`data`  

The data to send to `remote`.

`sendTimeout`  

The time to wait for `data` to be sent.

`rcvTimeout`  

The time to wait for a reply to be returned.

`replyMode`  

The run loop mode in which the function should wait for a reply. If the message is a `oneway` (so no response is expected), then `replyMode` should be `NULL`. If `replyMode` is non-`NULL`, the function runs the run loop waiting for a reply, in that mode. `replyMode` can be any string name of a run loop mode, but it should be one with input sources installed. You should use the `kCFRunLoopDefaultMode` constant unless you have a specific reason to use a different mode.

`returnData`  

Upon return, contains a CFData object containing the reply data. Ownership follows the The Create Rule.

## Return Value

Error code indicating success or failure. See CFMessagePortSendRequest Error Codes for the possible return values.

## See Also

### Using a Message Port

func CFMessagePortInvalidate(CFMessagePort!)

Invalidates a CFMessagePort object, stopping it from receiving or sending any more messages.

func CFMessagePortSetDispatchQueue(CFMessagePort!, dispatch_queue_t!)

Schedules callbacks for the specified message port on the specified dispatch queue.

