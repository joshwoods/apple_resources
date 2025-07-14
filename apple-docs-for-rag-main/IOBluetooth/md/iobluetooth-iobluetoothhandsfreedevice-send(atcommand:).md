

- IOBluetooth
- IOBluetoothHandsFreeDevice
-  send(atCommand:) 

Instance Method

# send(atCommand:)

Sends an AT command to the Bluetooth audio gateway.

macOS 10.7+

``` source
func send(atCommand: String!)
```

## Parameters 

`atCommand`  

A string containing the AT command.

## See Also

### Sending Messages and Commands

func sendSMS(String!, message: String!)

Sends a text message to a phone number.

func sendDTMF(String!)

Sends the tone associated with a phone key to the hands-free Bluetooth device.

func send(atCommand: String!, timeout: Float, selector: Selector!, target: Any!)

Send an AT command to the Bluetooth audio gateway and performs a selector on completion or timeout.

