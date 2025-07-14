

- IOBluetooth
- IOBluetoothHandsFreeAudioGateway
-  sendResponse(\_:withOK:) 

Instance Method

# sendResponse(\_:withOK:)

Sends data followed by an optional success message to a connected Bluetooth hands-free phone or headset.

macOS 10.7+

``` source
func sendResponse(
    _ response: String!,
    withOK: Bool
)
```

## Parameters 

`response`  

A string containing the data.

`withOK`  

If `true`, send an `OK` message after sending the response.

## See Also

### Sending and Receiving Commands

func sendResponse(String!)

Sends data followed by a success message to a connected Bluetooth hands-free phone or headset.

func sendOKResponse()

Sends a success message to a connected Bluetooth hands-free phone or headset.

func process(atCommand: String!)

Processes a command from a connected Bluetooth hands-free phone or headset.

