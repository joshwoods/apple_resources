

- IOBluetooth
- IOBluetoothHandsFreeAudioGateway
-  sendResponse(\_:) 

Instance Method

# sendResponse(\_:)

Sends data followed by a success message to a connected Bluetooth hands-free phone or headset.

macOS 10.7+

``` source
func sendResponse(_ response: String!)
```

## Parameters 

`response`  

A string containing the data.

## Discussion

Calling this method has the same result as calling `sendResponse(response: response, withOK: true)`.

## See Also

### Sending and Receiving Commands

func sendResponse(String!, withOK: Bool)

Sends data followed by an optional success message to a connected Bluetooth hands-free phone or headset.

func sendOKResponse()

Sends a success message to a connected Bluetooth hands-free phone or headset.

func process(atCommand: String!)

Processes a command from a connected Bluetooth hands-free phone or headset.

