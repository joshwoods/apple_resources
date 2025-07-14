

- IOBluetooth
- IOBluetoothHandsFreeDevice
-  memoryDial(\_:) 

Instance Method

# memoryDial(\_:)

Calls the phone number stored in a speed dial or memory slot of the hands-free phone or headset.

macOS 10.7+

``` source
func memoryDial(_ memoryLocation: Int32)
```

## Parameters 

`memoryLocation`  

The speed dial or other memory index of a phone number.

## See Also

### Dialing Calls

func dialNumber(String!)

Calls the phone number on a hands-free phone or headset.

func redial()

Calls the number stored on the hands-free phone or headset again.

