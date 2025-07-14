

- IOBluetooth
-  OBEXTransportEvent 

Structure

# OBEXTransportEvent

macOS

``` source
struct OBEXTransportEvent
```

## Overview

You will need to construcy these when data is received, and then pass a pointer to it to one of the incoming data methods defined below. Pass 0 as your status if data was received OK. Otherwise, you can put your own error code in there. For the transport type, be sure to use one of the defined types above.

## Topics

### Initializers

init()

init(type: OBEXTransportEventType, status: OBEXError, dataPtr: UnsafeMutableRawPointer!, dataLength: Int)

### Instance Properties

var dataLength: Int

var dataPtr: UnsafeMutableRawPointer!

var status: OBEXError

var type: OBEXTransportEventType

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### DataTypes

typealias OBEXTransportEventType

