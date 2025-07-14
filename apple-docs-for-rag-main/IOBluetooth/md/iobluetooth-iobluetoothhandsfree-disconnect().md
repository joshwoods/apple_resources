

- IOBluetooth
- IOBluetoothHandsFree
-  disconnect() 

Instance Method

# disconnect()

Disconnect from the device

macOS 10.7+

``` source
func disconnect()
```

## Discussion

Disconnects from the device, closes the SCO and service level connection if they are connected. Delegate methods will be called once the disconnection is complete.

