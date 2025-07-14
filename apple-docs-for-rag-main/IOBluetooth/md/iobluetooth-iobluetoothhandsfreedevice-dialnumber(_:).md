

- IOBluetooth
- IOBluetoothHandsFreeDevice
-  dialNumber(\_:) 

Instance Method

# dialNumber(\_:)

Calls the phone number on a hands-free phone or headset.

macOS 10.7+

``` source
func dialNumber(_ aNumber: String!)
```

## Parameters 

`aNumber`  

A string containing a phone number.

## See Also

### Dialing Calls

func memoryDial(Int32)

Calls the phone number stored in a speed dial or memory slot of the hands-free phone or headset.

func redial()

Calls the number stored on the hands-free phone or headset again.

