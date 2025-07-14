

- IOBluetooth
- OBEXSession
-  hasOpenOBEXConnection() 

Instance Method

# hasOpenOBEXConnection()

Has a successful connect packet been sent and received? This API tells you so.

macOS

``` source
func hasOpenOBEXConnection() -> Bool
```

## Return Value

True or false, we are OBEX-connected to another OBEX entity.

## Discussion

A “transport” connection may exist (such as a Bluetooth baseband connection), but the OBEX connection may not be established over that transport. If it has been, this function returns true.

