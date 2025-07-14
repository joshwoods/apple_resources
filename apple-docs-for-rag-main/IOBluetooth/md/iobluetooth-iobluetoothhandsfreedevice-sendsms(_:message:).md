

- IOBluetooth
- IOBluetoothHandsFreeDevice
-  sendSMS(\_:message:) 

Instance Method

# sendSMS(\_:message:)

Sends a text message to a phone number.

macOS 10.7+

``` source
func sendSMS(
    _ aNumber: String!,
    message aMessage: String!
)
```

## Parameters 

`aNumber`  

The phone number to send the message to.

`aMessage`  

A string containing a message. The message must be no longer than 160 characters.

## See Also

### Sending Messages and Commands

func sendDTMF(String!)

Sends the tone associated with a phone key to the hands-free Bluetooth device.

func send(atCommand: String!)

Sends an AT command to the Bluetooth audio gateway.

func send(atCommand: String!, timeout: Float, selector: Selector!, target: Any!)

Send an AT command to the Bluetooth audio gateway and performs a selector on completion or timeout.

