

- Background Assets
- BADownload
-  BADownload.State 

Enumeration

# BADownload.State

Constants that indicate the state of a download.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum State
```

## Topics

### Download states

case created

A state that indicates a created download.

case waiting

A state that indicates a download is waiting to execute.

case downloading

A state that indicates a download is in progress.

case finished

A state that indicates a finished download.

case failed

A state that indicates a failed download.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the current state

var state: BADownload.State

The current state of the download.

