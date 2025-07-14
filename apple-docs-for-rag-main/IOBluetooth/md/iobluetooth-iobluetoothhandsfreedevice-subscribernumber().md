

- IOBluetooth
- IOBluetoothHandsFreeDevice
-  subscriberNumber() 

Instance Method

# subscriberNumber()

Requests that the Bluetooth audio gateway send the subscriber number to the delegate.

macOS 10.7+

``` source
func subscriberNumber()
```

## Discussion

The subscriber number is sent to the handsFree(_:subscriberNumber:) function of the delegate.

## See Also

### Requesting Status Information

func currentCallList()

Requests that the Bluetooth audio gateway send the delegate a list of calls that are active, on hold, or being set up.

