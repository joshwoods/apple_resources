

- Dispatch
-  DispatchSourceSignal 

Protocol

# DispatchSourceSignal

A dispatch source that monitors the current process for UNIX signals.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol DispatchSourceSignal : DispatchSourceProtocol, Sendable
```

## Overview

You do not adopt this protocol in your objects. Instead, use the makeSignalSource(signal:queue:) method to create an object that adopts this protocol.

## Relationships

### Inherits From

- DispatchSourceProtocol
- NSObjectProtocol
- Sendable

### Conforming Types

- DispatchSource

## See Also

### Creating a Signal Source

class func makeSignalSource(signal: Int32, queue: DispatchQueue?) -> any DispatchSourceSignal

Creates a new dispatch source object that monitors the arrival of a UNIX signal.

