

- Core NFC
- CardSession
-  stopEmulation(status:) 

Instance Method

# stopEmulation(status:)

Stop card emulation and display a status.

iOS 17.4+iPadOS 17.4+

``` source
func stopEmulation(status: CardSession.EmulationUIStatus) async
```

## Parameters 

`status`  

The final status to display.

## See Also

### Managing card emulation

func startEmulation() async throws

Start the card emulation and present a modal user interface to the person using the app.

enum Error

An error type that indicates problems with a card session.

enum EmulationUIStatus

The final status to show in the user interface when ending card emulation.

var isEmulationInProgress: Bool

A Boolean value that indicates whether emulation is currently active.

