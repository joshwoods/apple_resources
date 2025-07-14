

- IOBluetooth
- IOBluetoothHandsFreeAudioGateway
-  sendOKResponse() 

Instance Method

# sendOKResponse()

Sends a success message to a connected Bluetooth hands-free phone or headset.

macOS 10.7+

``` source
func sendOKResponse()
```

## See Also

### Sending and Receiving Commands

func sendResponse(String!)

Sends data followed by a success message to a connected Bluetooth hands-free phone or headset.

func sendResponse(String!, withOK: Bool)

Sends data followed by an optional success message to a connected Bluetooth hands-free phone or headset.

func process(atCommand: String!)

Processes a command from a connected Bluetooth hands-free phone or headset.

