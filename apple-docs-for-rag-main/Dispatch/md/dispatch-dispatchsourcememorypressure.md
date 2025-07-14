

- Dispatch
-  DispatchSourceMemoryPressure 

Protocol

# DispatchSourceMemoryPressure

A dispatch source that monitors the system for changes in the memory pressure condition.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol DispatchSourceMemoryPressure : DispatchSourceProtocol, Sendable
```

## Overview

You do not adopt this protocol in your objects. Instead, use the makeMemoryPressureSource(eventMask:queue:) method to create an object that adopts this protocol.

## Topics

### Getting the Event Data

var data: DispatchSource.MemoryPressureEvent

var mask: DispatchSource.MemoryPressureEvent

## Relationships

### Inherits From

- DispatchSourceProtocol
- NSObjectProtocol
- Sendable

### Conforming Types

- DispatchSource

## See Also

### Creating a Memory Pressure Source

class func makeMemoryPressureSource(eventMask: DispatchSource.MemoryPressureEvent, queue: DispatchQueue?) -> any DispatchSourceMemoryPressure

Creates a new dispatch source object that monitors the system for changes in the memory pressure condition.

struct MemoryPressureEvent

Memory pressure events.

