

- IOBluetooth
- IOBluetoothHandsFreeDevice
-  currentCallList() 

Instance Method

# currentCallList()

Requests that the Bluetooth audio gateway send the delegate a list of calls that are active, on hold, or being set up.

macOS 10.7+

``` source
func currentCallList()
```

## Discussion

The handsFree(_:currentCall:) function of the delegate is called once for each current call.

## See Also

### Requesting Status Information

func subscriberNumber()

Requests that the Bluetooth audio gateway send the subscriber number to the delegate.

