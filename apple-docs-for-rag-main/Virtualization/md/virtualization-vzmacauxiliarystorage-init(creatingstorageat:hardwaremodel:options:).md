

- Virtualization
- VZMacAuxiliaryStorage
-  init(creatingStorageAt:hardwareModel:options:) 

Initializer

# init(creatingStorageAt:hardwareModel:options:)

Creates an initialized Mac auxiliary storage instance that describes a specific hardware model at a URL you specify.

macOS 12.0+

``` source
init(
    creatingStorageAt URL: URL,
    hardwareModel: VZMacHardwareModel,
    options: VZMacAuxiliaryStorage.InitializationOptions = []
) throws
```

## Parameters 

`URL`  

The `URL` to write the auxiliary storage to on the local file system.

`hardwareModel`  

The VZMacHardwareModel model to use. The auxiliary storage can have different layouts for different hardware models.

`options`  

Initialization options from the available VZMacAuxiliaryStorage.InitializationOptions.

## Return Value

Returns a newly initialized `VZMacAuxiliaryStorage` object on success or `nil` if there was an error. On failure, `error` contains the `NSError` that describes reason for the failure.

## Mentioned in 

Installing macOS on a Virtual Machine

## Discussion

Use this method to create a new auxiliary storage object that describes a specific hardware model. To restore data from a previously saved existing auxiliary storage object, use init(contentsOfURL:).

## See Also

### Creating the auxiliary storage

init(contentsOfURL: URL)

Initializes an auxiliary storage object with data from the location at the URL you provide.

Deprecated

init(url: URL)

Initializes an auxiliary storage object with data from the location at the URL you provide.

struct InitializationOptions

Options you can set when creating new auxiliary storage.

