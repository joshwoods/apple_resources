

- Kernel
- Hardware Families
- Network
- IONetworkData
-  writeBytes 

# writeBytes

Writes to the data buffer with data from a source buffer provided by the caller.

``` source
virtual bool writeBytes(
 const void *srcBuffer, 
 UInt32 srcBufferSize, 
 UInt32 writeOffset = 0); 
```

## Parameters 

`srcBuffer`  

Pointer to a source buffer provided by the caller.

`srcBufferSize`  

The size of the source buffer.

`writeOffset`  

A byte offset from the start of the data buffer to begin writting.

## Return Value

Returns true if the operation was successful, false otherwise.

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

