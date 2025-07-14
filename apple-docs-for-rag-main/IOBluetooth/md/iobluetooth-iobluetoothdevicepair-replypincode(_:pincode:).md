

- IOBluetooth
- IOBluetoothDevicePair
-  replyPINCode(\_:pinCode:) 

Instance Method

# replyPINCode(\_:pinCode:)

This is the required reply to the devicePairingPINCodeRequest delegate message. Set the PIN code to use during pairing if required.

macOS

``` source
func replyPINCode(
    _ PINCodeSize: Int,
    pinCode PINCode: UnsafeMutablePointer!
)
```

## Parameters 

`PINCodeSize`  

The PIN code length in octets (8 bits).

`PINCode`  

PIN code for the device. Can be up to a maximum of 128 bits.

