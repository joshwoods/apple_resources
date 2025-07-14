

- SerialDriverKit
- IOUserSerial
-  initWith 

Instance Method

# initWith

Initializes the private data structures associated with this class.

DriverKit 19.0+

``` source
bool initWith(IOBufferMemoryDescriptor * ifmd);
```

## Parameters 

`ifmd`  

The memory buffer to use for interrupt-related data.

## Return Value

`YES` if initialization succeeded, or `NO` if it didn’t.

## Discussion

Do not override or call this method. Instead, override the init method and use it to allocate memory for your driver’s data structures.

## See Also

### Configuring the Service

init

Handles the basic initialization of the service.

Start

Starts the current service and associates it with the specified provider.

Stop

Stops the service associated with the specified provider.

free

Performs any final cleanup for the service.

