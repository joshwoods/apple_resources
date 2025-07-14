

- IOBluetooth
- IOBluetoothDevice
-  remoteNameRequest(\_:withPageTimeout:) 

Instance Method

# remoteNameRequest(\_:withPageTimeout:)

Issues a remote name request to the target device.

macOS

``` source
func remoteNameRequest(
    _ target: Any!,
    withPageTimeout pageTimeoutValue: BluetoothHCIPageTimeout
) -> IOReturn
```

## Parameters 

`target`  

The target to message when the remote name request is complete

`pageTimeoutValue`  

The page timeout value to use for this call

## Return Value

Returns kIOReturnSuccess if the remote name request was successfully issued (and if synchronous, if the request completed successfully).

## Discussion

If a target is specified, the request is asynchronous and on completion of the REMOTE_NAME_REQUEST command, the method -remoteNameRequestComplete:status:name: will be called on the specified target. If no target is specified, the request is made synchronously and won’t return until the request is complete.

NOTE: This method is only available in macOS 10.2.7 (Bluetooth v1.3) or later.

