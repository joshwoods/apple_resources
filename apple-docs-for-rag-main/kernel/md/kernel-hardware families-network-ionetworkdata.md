

- Kernel
- Hardware Families
- Network
-  IONetworkData 

Class

# IONetworkData

An object that manages a fixed-size named buffer.

macOS 10.6+

``` source
class IONetworkData : OSObject
```

## Overview

An IONetworkData object manages a fixed-size named buffer. This object provides external access methods that can be used to access the contents of the data buffer. In addition, serialization is supported, and therefore this object can be added to a property table to publish the data object. An unique name must be assigned to the object during initialization. An OSSymbol key will be created based on the assigned name, and this key can be used when the object is added to a dictionary.

The level of access granted to the access methods can be restricted, by specifying a set of supported access types when the object is initialized, or modified later by calling setAccessTypes(). By default, each IONetworkData object created will support serialization, and will also allow its data buffer to be read through the read() access method.

An access notification handler, in the form of a 'C' function, can be registered to receive a call each time the data buffer is accessed through an access method. Arguments provided to the handler will identify the data object and the type of access that triggered the notification. The handler can therefore perform lazy update of the data buffer until an interested party tries to read or serialize the data. The notification handler can also take over the default action performed by the access methods when the buffer type is set to kIONetworkDataBufferTypeNone. This will prevent the access methods from accessing the data buffer, and allow the handler to override the access protocol.

This object is primarily used by IONetworkInterface to export interface properties to user space.

## Topics

### Miscellaneous

clearBuffer

Clears the data buffer by filling it with zeroes.

free

Frees the IONetworkData object.

getAccessTypes

Gets the types of data access supported by this object.

getBuffer

Gets a pointer to the data buffer.

getBufferType

Gets the type of data buffer managed by this object.

getKey

Gets a unique OSSymbol key associated with this object.

getNotificationAction

Gets the C function that was registered to handle access notifications sent from this object.

getNotificationParameter

Gets the parameter that will be passed to the access notification handler.

getNotificationTarget

Gets the first parameter that will be passed to the access notification handler.

getSize

Gets the size of the data buffer.

init

Initializes an IONetworkData object.

read

An access method that reads from the data buffer.

readBytes

Reads from the data buffer and copies the data to a destination buffer provided by the caller.

reset

An access method that resets the data buffer.

serialize

Serializes the IONetworkData object.

setAccessTypes

Sets the types of access that are permitted on the data buffer.

setNotificationTarget

Registers a C function to handle access notifications sent from this object.

withExternalBuffer

Factory method that constructs and initializes an IONetworkData object with an external data buffer.

withInternalBuffer

Factory method that constructs and initializes an IONetworkData object with an internal data buffer.

withNoBuffer

Factory method that constructs and initializes an IONetworkData object without a data buffer.

write

An access method that writes to the data buffer.

writeBytes

Writes to the data buffer with data from a source buffer provided by the caller.

### Callbacks

Action

### Instance Variables

_reserved

### Instance Methods

- clearBuffer

- free

- getAccessTypes

- getBuffer

- getBufferType

- getKey

- getMetaClass

- getNotificationAction

- getNotificationParameter

- getNotificationTarget

- getSize

- init

- read

- readBytes

- reset

- serialize

- setAccessTypes

- setNotificationTarget

- write

- writeBytes

### Type Methods

+ withExternalBuffer

+ withInternalBuffer

+ withNoBuffer

## Relationships

### Inherits From

- OSObject

## See Also

### Network Data

IONetworkMedium

An object that encapsulates information about a network medium (i.e. 10Base-T, or 100Base-T Full Duplex).

IOPacketQueue

Implements a bounded FIFO queue of mbuf packets.

IOPacketBufferConstraints

