

- DriverKit
- IOMemoryDescriptor
-  init 

Instance Method

# init

Initializes the memory descriptor object.

DriverKitiOSiPadOSmacOS

``` source
bool init();
```

## Return Value

true if initialization was successful, or false if it was unsuccessful.

## Discussion

Don’t call this method directly. To allocate a memory buffer for your driver, call the Create method of IOBufferMemoryDescriptor.

## See Also

### Configuring the Buffer

free

Performs any final cleanup for the memory descriptor object.

