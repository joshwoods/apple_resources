

- IOBluetooth
- IOBluetoothHandsFreeDevice
-  placeAllOthers(onHold:) 

Instance Method

# placeAllOthers(onHold:)

Places all calls except the call with the specified index on hold.

macOS 10.7+

``` source
func placeAllOthers(onHold index: Int32)
```

## Parameters 

`index`  

The index of the call that remains active.

## See Also

### Holding Calls

func holdCall()

Places all active calls on hold and accepts a held or waiting call.

func addHeldCall()

Adds held calls to the current conversation.

