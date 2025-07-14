

- IOBluetooth
- IOBluetoothHandsFreeAudioGateway
-  process(atCommand:) 

Instance Method

# process(atCommand:)

Processes a command from a connected Bluetooth hands-free phone or headset.

macOS 10.7+

``` source
func process(atCommand: String!)
```

## Parameters 

`atCommand`  

A string containing the AT command sent from the hands-free Bluetooth device.

## See Also

### Sending and Receiving Commands

func sendResponse(String!)

Sends data followed by a success message to a connected Bluetooth hands-free phone or headset.

func sendResponse(String!, withOK: Bool)

Sends data followed by an optional success message to a connected Bluetooth hands-free phone or headset.

func sendOKResponse()

Sends a success message to a connected Bluetooth hands-free phone or headset.

