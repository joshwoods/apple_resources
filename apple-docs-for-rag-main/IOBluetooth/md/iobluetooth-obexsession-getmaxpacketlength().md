

- IOBluetooth
- OBEXSession
-  getMaxPacketLength() 

Instance Method

# getMaxPacketLength()

Gets current max packet length.

macOS

``` source
func getMaxPacketLength() -> OBEXMaxPacketLength
```

## Return Value

Max packet length.

## Discussion

This value *could* change before and after a connect command has been sent or a connect command response has been received, since the recipient could negotiate a lower max packet size.

