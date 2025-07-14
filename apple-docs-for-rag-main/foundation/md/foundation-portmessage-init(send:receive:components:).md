

- Foundation
- PortMessage
-  init(send:receive:components:) 

Initializer

# init(send:receive:components:)

Initializes a newly allocated `NSPortMessage` object to send given data on a given port and to receiver replies on another given port.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(
    send sendPort: Port?,
    receive replyPort: Port?,
    components: [Any]?
)
```

## Parameters 

`sendPort`  

The port on which the message is sent.

`replyPort`  

The port on which replies to the message arrive.

`components`  

The data to send in the message. `components` should contain only `NSData` and `NSPort` objects, and the contents of the `NSData` objects should be in network byte order.

## Return Value

An `NSPortMessage` object initialized to send `components` on `sendPort` and to receiver replies on `receivePort`.

## Discussion

An `NSPortMessage` object initialized with this method has a message identifier of 0.

This is the designated initializer for `NSPortMessage`.

## See Also

### Related Documentation

var msgid: UInt32

Returns the identifier for the receiver.

Distributed Objects Programming Topics

