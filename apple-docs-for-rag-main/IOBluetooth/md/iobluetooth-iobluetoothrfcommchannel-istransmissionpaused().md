

- IOBluetooth
- IOBluetoothRFCOMMChannel
-  isTransmissionPaused() 

Instance Method

# isTransmissionPaused()

Returns TRUE if flow control is off.

macOS

``` source
func isTransmissionPaused() -> Bool
```

## Return Value

TRUE if the action of sending data will block the current thread, FALSE otherwise.

## Discussion

Returns true if the remote device flow control is stopping out transmission. This is useful because we do not buffer data, we stop the transmitting actor. With this method the transmitter can check if sending data is going to be successful or is going to block.

