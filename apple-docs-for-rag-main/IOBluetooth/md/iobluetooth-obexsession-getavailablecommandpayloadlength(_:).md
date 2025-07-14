

- IOBluetooth
- OBEXSession
-  getAvailableCommandPayloadLength(\_:) 

Instance Method

# getAvailableCommandPayloadLength(\_:)

Determine the maximum amount of data you can send in a particular command as an OBEX client session.

macOS

``` source
func getAvailableCommandPayloadLength(_ inOpCode: OBEXOpCode) -> OBEXMaxPacketLength
```

## Parameters 

`inOpCode`  

The opcode you are interested in sending (as a client).

## Return Value

The maximum amount of data a particular packet can handle, after accounting for any command overhead.

## Discussion

Each OBEX Command has a certain amount of overhead. Since the negotiated max packet length does not indicate what the maximum data amount you can send in a particular command’s packet, you can use this function to determine how much data to provide in optional headers or body data headers.

