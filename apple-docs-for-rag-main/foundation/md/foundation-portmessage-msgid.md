

- Foundation
- PortMessage
-  msgid 

Instance Property

# msgid

Returns the identifier for the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
var msgid: UInt32 { get set }
```

## Return Value

The identifier for the receiver.

## Discussion

Cooperating applications can use this to define different types of messages, such as connection requests, RPCs, errors, and so on.

