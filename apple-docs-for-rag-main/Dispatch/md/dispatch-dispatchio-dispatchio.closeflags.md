

- Dispatch
- DispatchIO
-  DispatchIO.CloseFlags 

Structure

# DispatchIO.CloseFlags

Additional flags to use when closing an I/O channel.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CloseFlags
```

## Topics

### Close Flags

static let stop: DispatchIO.CloseFlags

Stop any in-progress read/write operations when closed.

### Initializing the Type

var DISPATCH_IO_STOP: Int32

Stop any in-progress read and write operations when closed.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Closing the File

func close(flags: DispatchIO.CloseFlags)

Closes the channel to new read and write operations.

