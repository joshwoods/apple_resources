

- Virtualization
- VZEFIVariableStore
-  init(creatingVariableStoreAt:options:) 

Initializer

# init(creatingVariableStoreAt:options:)

Creates a new EFI variable store at specified the URL on the filesystem, initialization options, and error-return variable.

macOS 13.0+

``` source
init(
    creatingVariableStoreAt URL: URL,
    options: VZEFIVariableStore.InitializationOptions = []
) throws
```

## Parameters 

`URL`  

A URL that specifies the location on disk at which to store the EFI information.

`options`  

An array of possible VZEFIVariableStore.InitializationOptions.

## See Also

### Creating the variable store

init(url: URL)

Initialize the variable store from the URL of an existing file.

struct InitializationOptions

Constants that describe the options available when creating a new Extensible Firmware Interface (EFI) variable store.

