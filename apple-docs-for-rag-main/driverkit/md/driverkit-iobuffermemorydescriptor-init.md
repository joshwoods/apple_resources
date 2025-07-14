

- DriverKit
- IOBufferMemoryDescriptor
-  init 

Instance Method

# init

Initializes the buffer memory descriptor object.

DriverKitiOSiPadOSmacOS

``` source
bool init();
```

## Return Value

`true` if initialization was successful, or `false` if it was unsuccessful.

## Discussion

Don’t call this method directly. Use the Create method instead.

## See Also

### Creating a Memory Buffer

Create

Creates a new memory buffer descriptor object in the current process space.

free

Performs any final cleanup for the memory buffer descriptor object.

