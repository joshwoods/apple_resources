

- Dispatch
-  DispatchSourceProcess 

Protocol

# DispatchSourceProcess

A dispatch source that monitors an external process for events.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol DispatchSourceProcess : DispatchSourceProtocol, Sendable
```

## Overview

You do not adopt this protocol in your objects. Instead, use the makeProcessSource(identifier:eventMask:queue:) method to create an object that adopts this protocol.

## Topics

### Getting the Process ID

var handle: pid_t

The process identifier of the process being monitored by the dispatch source.

### Getting the Event Data

var data: DispatchSource.ProcessEvent

Data associated with the last process-related event.

var mask: DispatchSource.ProcessEvent

The process events being monitored by the dispatch source.

## Relationships

### Inherits From

- DispatchSourceProtocol
- NSObjectProtocol
- Sendable

### Conforming Types

- DispatchSource

## See Also

### Creating a Process Source

class func makeProcessSource(identifier: pid_t, eventMask: DispatchSource.ProcessEvent, queue: DispatchQueue?) -> any DispatchSourceProcess

Creates a new dispatch source object for monitoring the specified process.

struct ProcessEvent

Events related to a process.

