

- Virtualization
- VZEFIVariableStore
-  init(url:) 

Initializer

# init(url:)

Initialize the variable store from the URL of an existing file.

macOS 13.0+

``` source
init(url URL: URL)
```

## Parameters 

`URL`  

The URL of the location on disk that contains the stored EFI information.

## See Also

### Creating the variable store

init(creatingVariableStoreAt: URL, options: VZEFIVariableStore.InitializationOptions) throws

Creates a new EFI variable store at specified the URL on the filesystem, initialization options, and error-return variable.

struct InitializationOptions

Constants that describe the options available when creating a new Extensible Firmware Interface (EFI) variable store.

