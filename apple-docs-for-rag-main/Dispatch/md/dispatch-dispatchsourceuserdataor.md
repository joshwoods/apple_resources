

- Dispatch
-  DispatchSourceUserDataOr 

Protocol

# DispatchSourceUserDataOr

A dispatch source that coalesces data you provide using an OR operation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol DispatchSourceUserDataOr : DispatchSourceProtocol, Sendable
```

## Overview

You do not adopt this protocol in your objects. Instead, use the makeUserDataOrSource(queue:) method to create an object that adopts this protocol.

To add custom data to the dispatch source, call the or(data:) method.

## Topics

### Getting the Event Data

func or(data: UInt)

## Relationships

### Inherits From

- DispatchSourceProtocol
- NSObjectProtocol
- Sendable

### Conforming Types

- DispatchSource

## See Also

### Creating a Custom Source

class func makeUserDataAddSource(queue: DispatchQueue?) -> any DispatchSourceUserDataAdd

Creates a new dispatch source object that you use to coalesce custom app data using an AND operator.

class func makeUserDataOrSource(queue: DispatchQueue?) -> any DispatchSourceUserDataOr

Creates a new dispatch source object that you use to coalesce custom app data using an OR operator.

class func makeUserDataReplaceSource(queue: DispatchQueue?) -> any DispatchSourceUserDataReplace

Creates a new dispatch source object that you use to track custom app data.

protocol DispatchSourceUserDataAdd

A dispatch source that coalesces data you provide using an AND operation.

protocol DispatchSourceUserDataReplace

A dispatch source that replaces any pending data with the new value you provide.

