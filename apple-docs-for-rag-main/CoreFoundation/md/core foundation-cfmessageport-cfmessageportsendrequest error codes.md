

- Core Foundation
- CFMessagePort
-  CFMessagePortSendRequest Error Codes 

API Collection

# CFMessagePortSendRequest Error Codes

Error codes for `CFMessagePortSendRequest`.

## Topics

### Constants

var kCFMessagePortSuccess: Int32

The message was successfully sent and, if a reply was expected, a reply was received.

var kCFMessagePortSendTimeout: Int32

The message could not be sent before the send timeout.

var kCFMessagePortReceiveTimeout: Int32

No reply was received before the receive timeout.

var kCFMessagePortIsInvalid: Int32

The message could not be sent because the message port is invalid.

var kCFMessagePortTransportError: Int32

An error occurred trying to send the message.

var kCFMessagePortBecameInvalidError: Int32

The message port was invalidated.

