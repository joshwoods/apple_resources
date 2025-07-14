

- Virtualization
- VZMacAuxiliaryStorage
-  init(url:) 

Initializer

# init(url:)

Initializes an auxiliary storage object with data from the location at the URL you provide.

macOS 13.0+

``` source
init(url URL: URL)
```

## Parameters 

`URL`  

The URL of the auxiliary storage on the local file system.

## See Also

### Creating the auxiliary storage

init(contentsOfURL: URL)

Initializes an auxiliary storage object with data from the location at the URL you provide.

Deprecated

init(creatingStorageAt: URL, hardwareModel: VZMacHardwareModel, options: VZMacAuxiliaryStorage.InitializationOptions) throws

Creates an initialized Mac auxiliary storage instance that describes a specific hardware model at a URL you specify.

struct InitializationOptions

Options you can set when creating new auxiliary storage.

