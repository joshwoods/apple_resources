

- Core NFC
- CardSession
-  isEmulationInProgress 

Instance Property

# isEmulationInProgress

A Boolean value that indicates whether emulation is currently active.

iOS 17.4+iPadOS 17.4+

``` source
var isEmulationInProgress: Bool { get async }
```

## See Also

### Managing card emulation

func startEmulation() async throws

Start the card emulation and present a modal user interface to the person using the app.

enum Error

An error type that indicates problems with a card session.

func stopEmulation(status: CardSession.EmulationUIStatus) async

Stop card emulation and display a status.

enum EmulationUIStatus

The final status to show in the user interface when ending card emulation.

