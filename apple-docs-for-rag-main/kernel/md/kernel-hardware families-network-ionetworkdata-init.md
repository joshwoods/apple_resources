

- Kernel
- Hardware Families
- Network
- IONetworkData
-  init 

# init

Initializes an IONetworkData object.

``` source
virtual bool init(
 const char *name, 
 UInt32 bufferType, 
 UInt32 bufferSize, 
 void *externalBuffer = 0, 
 UInt32 accessTypes = (
 kIONetworkDataAccessTypeRead | kIONetworkDataAccessTypeSerialize), 
 void *target = 0, 
 Action action = 0, 
 void *param = 0); 
```

## Parameters 

`name`  

A name to assign to this object.

`bufferType`  

The type of buffer associated with this object.

`bufferSize`  

The size of the data buffer.

`externalBuffer`  

Pointer to an external data buffer.

`accessTypes`  

The initial supported access types. Can be later modified by calling setAccessTypes().

`target`  

The notification target.

`action`  

The notification action.

`param`  

A parameter to pass to the notification action.

## Return Value

Returns true if initialized successfully, false otherwise.

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

