

- IOBluetooth
- OBEXSession
-  closeTransportConnection() 

Instance Method

# closeTransportConnection()

You must override this - it will be called when the transport connection should be shutdown.

macOS

``` source
func closeTransportConnection() -> OBEXError
```

## Return Value

Return whether or not the transport connection was closed successfully or not. Return OBEXSuccess ( 0 ) on success, otherwise an error code.

## Discussion

Tranport subclasses must override this! When called you should take whatever steps are necessary to actually close down the transport connection.

