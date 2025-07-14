

- IOBluetooth
- IOBluetoothDevice
-  getServiceRecord(for:) 

Instance Method

# getServiceRecord(for:)

Search for a service record containing the given UUID.

macOS

``` source
func getServiceRecord(for sdpUUID: IOBluetoothSDPUUID!) -> IOBluetoothSDPServiceRecord!
```

## Parameters 

`sdpUUID`  

UUID value to search for.

## Return Value

Returns the first service record that contains the given uuid. If no service record is found, nil is returned.

## Discussion

This method searches through the device’s services to find a service that contains the given UUID. Only the first service record will be returned. This method only operates on services that have already been queried. It will not initiate a new query. This method should probably be updated to return an array of service records if more than one contains the UUID.

