

- IOBluetooth
- IOBluetoothHandsFree
-  connect() 

Instance Method

# connect()

Connect to the device

macOS 10.7+

``` source
func connect()
```

## Discussion

Connects to the device and sets up a service level connection (RFCOMM channel). Delegate methods will be called once the connection is complete or a failure occurs.

