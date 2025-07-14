

- IOBluetooth
- IOBluetoothHandsFreeDevice
-  sendDTMF(\_:) 

Instance Method

# sendDTMF(\_:)

Sends the tone associated with a phone key to the hands-free Bluetooth device.

macOS 10.7+

``` source
func sendDTMF(_ character: String!)
```

## Parameters 

`character`  

The phone keypad character for the tone. The character must be one of the following:

- `0-9`

- `#`

- `*`

- `A-D`

## See Also

### Sending Messages and Commands

func sendSMS(String!, message: String!)

Sends a text message to a phone number.

func send(atCommand: String!)

Sends an AT command to the Bluetooth audio gateway.

func send(atCommand: String!, timeout: Float, selector: Selector!, target: Any!)

Send an AT command to the Bluetooth audio gateway and performs a selector on completion or timeout.

