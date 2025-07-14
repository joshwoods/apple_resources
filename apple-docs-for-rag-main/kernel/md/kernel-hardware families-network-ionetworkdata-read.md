

- Kernel
- Hardware Families
- Network
- IONetworkData
-  read 

# read

An access method that reads from the data buffer.

``` source
virtual IOReturn read(
 void *dstBuffer, 
 UInt32 *dstBufferSize, 
 UInt32 readOffset = 0); 
```

## Parameters 

`dstBuffer`  

Pointer to the destination buffer.

`dstBufferSize`  

Pointer to an integer containing the size of the destination buffer. And is overwritten by this method to the actual number of bytes copied to the destination buffer.

`readOffset`  

An offset from the start of the source data buffer to begin reading.

## Return Value

Returns kIOReturnSuccess on success, kIOReturnBadArgument if any of the arguments provided is invalid, kIOReturnNotReadable if read access is not permitted, or an error from the notification handler.

## Overview

This method handles an external request to read from the data buffer and copy it to the destination buffer provided by the accessor. If notification is enabled, then the notification handler is called before the data buffer is copied to the destination buffer. The notification handler may use this opportunity to intervene and to update the contents of the data buffer.

## See Also

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

