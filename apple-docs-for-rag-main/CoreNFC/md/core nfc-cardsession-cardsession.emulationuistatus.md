

- Core NFC
- CardSession
-  CardSession.EmulationUIStatus 

Enumeration

# CardSession.EmulationUIStatus

The final status to show in the user interface when ending card emulation.

iOS 17.4+iPadOS 17.4+

``` source
enum EmulationUIStatus
```

## Topics

### Emulation statuses

case success

A status display to indicate a successful operation, such as a checkmark.

case failure

A status display to indicate an error, such as an exclamation mark.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Managing card emulation

func startEmulation() async throws

Start the card emulation and present a modal user interface to the person using the app.

enum Error

An error type that indicates problems with a card session.

func stopEmulation(status: CardSession.EmulationUIStatus) async

Stop card emulation and display a status.

var isEmulationInProgress: Bool

A Boolean value that indicates whether emulation is currently active.

