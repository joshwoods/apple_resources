

- Virtualization
- VZMacAuxiliaryStorage
-  init(contentsOfURL:) Deprecated

Initializer

# init(contentsOfURL:)

Initializes an auxiliary storage object with data from the location at the URL you provide.

macOS 12.0–15.4Deprecated

``` source
init(contentsOfURL URL: URL)
```

``` source
init(contentsOf URL: URL)
```

## Parameters 

`URL`  

The URL of the auxiliary storage on the local file system.

## Discussion

Use this initializer to load the data from an auxiliary storage object stored on the file system. To create a new auxiliary storage object, use init(creatingStorageAt:hardwareModel:options:).

## See Also

### Creating the auxiliary storage

init(url: URL)

Initializes an auxiliary storage object with data from the location at the URL you provide.

init(creatingStorageAt: URL, hardwareModel: VZMacHardwareModel, options: VZMacAuxiliaryStorage.InitializationOptions) throws

Creates an initialized Mac auxiliary storage instance that describes a specific hardware model at a URL you specify.

struct InitializationOptions

Options you can set when creating new auxiliary storage.

