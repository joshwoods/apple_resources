

- IOBluetooth
- IOBluetoothDevice
-  remoteNameRequest(\_:) 

Instance Method

# remoteNameRequest(\_:)

Issues a remote name request to the target device.

macOS

``` source
func remoteNameRequest(_ target: Any!) -> IOReturn
```

## Parameters 

`target`  

The target to message when the remote name request is complete

## Return Value

Returns kIOReturnSuccess if the remote name request was successfully issued (and if synchronous, if the request completed successfully).

## Discussion

If a target is specified, the request is asynchronous and on completion of the request, the method

- (void)remoteNameRequestComplete:(IOBluetoothDevice \*)device status:(IOReturn)status;

will be called on the specified target. If no target is specified, the request is made synchronously and won’t return until the request is complete. This call with operate with the default page timeout value. If a different page timeout value is desired, the method -remoteNameRequest:withPageTimeout: should be used instead.

