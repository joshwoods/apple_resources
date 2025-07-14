

- IOBluetooth
- IOBluetoothHandsFree
-  connectSCO() 

Instance Method

# connectSCO()

Open a SCO connection with the device

macOS 10.7+

``` source
func connectSCO()
```

## Discussion

Opens a SCO connection with the device. The device must already have a service level connection or this will return immediately. Delegate methods will be called once the connection is complete of a failure occurs.

