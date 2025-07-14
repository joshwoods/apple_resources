

- DriverKit
- IOMemoryMap
-  init 

Instance Method

# init

Initializes the memory map object.

DriverKitiOSiPadOSmacOS

``` source
bool init();
```

## Return Value

`true` if initialization was successful, or `false` if it was unsuccessful.

## Discussion

Don’t call this method directly. To create a memory map object, call the CreateMapping method of IOMemoryDescriptor.

## See Also

### Configuring the Memory Map

free

Performs any final cleanup for the memory map object.

