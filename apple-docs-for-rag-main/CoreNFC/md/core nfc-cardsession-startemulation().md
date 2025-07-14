

- Core NFC
- CardSession
-  startEmulation() 

Instance Method

# startEmulation()

Start the card emulation and present a modal user interface to the person using the app.

iOS 17.4+iPadOS 17.4+

``` source
func startEmulation() async throws
```

## Discussion

Set the alertMessage prior to calling this method.

This method throws an error of type CardSession.Error if card emulation fails. Possible error conditions are:

- CardSession.Error.systemNotAvailable

- CardSession.Error.accessNotAccepted

- CardSession.Error.systemEligibilityFailed

- CardSession.Error.radioDisabled

## See Also

### Managing card emulation

enum Error

An error type that indicates problems with a card session.

func stopEmulation(status: CardSession.EmulationUIStatus) async

Stop card emulation and display a status.

enum EmulationUIStatus

The final status to show in the user interface when ending card emulation.

var isEmulationInProgress: Bool

A Boolean value that indicates whether emulation is currently active.

