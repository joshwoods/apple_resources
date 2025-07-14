

- IOBluetooth
- IOBluetoothHandsFreeDevice
-  send(atCommand:timeout:selector:target:) 

Instance Method

# send(atCommand:timeout:selector:target:)

Send an AT command to the Bluetooth audio gateway and performs a selector on completion or timeout.

macOS 10.7+

``` source
func send(
    atCommand: String!,
    timeout: Float,
    selector: Selector!,
    target: Any!
)
```

## Parameters 

`atCommand`  

A string containing the AT command.

`timeout`  

The number of seconds until the message times out.

`selector`  

The function to call on completion or timeout.

`target`  

The target object for the completion call.

## See Also

### Sending Messages and Commands

func sendSMS(String!, message: String!)

Sends a text message to a phone number.

func sendDTMF(String!)

Sends the tone associated with a phone key to the hands-free Bluetooth device.

func send(atCommand: String!)

Sends an AT command to the Bluetooth audio gateway.

