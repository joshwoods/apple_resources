

- Core Foundation
-  CFStreamError 

Structure

# CFStreamError

The structure returned by CFReadStreamGetError(_:) and CFWriteStreamGetError(_:).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFStreamError
```

## Topics

### Initializers

init()

init(domain: CFIndex, error: Int32)

### Instance Properties

var domain: CFIndex

The error domain that should be used to interpret the error. See CFStreamErrorDomain for possible values.

Deprecated

var error: Int32

The error code.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

struct CFStreamClientContext

A structure that contains program-defined data and callbacks with which you can configure a stream’s client behavior.

