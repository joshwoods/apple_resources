

- AppKit
- NSFilePromiseProvider
-  init(fileType:delegate:) 

Initializer

# init(fileType:delegate:)

Initializes a file promise provider for a certain file type.

macOS 10.12+

``` source
convenience init(
    fileType: String,
    delegate: any NSFilePromiseProviderDelegate
)
```

## Parameters 

`fileType`  

A string describing the file type.

`delegate`  

An object that conforms to the NSFilePromiseProviderDelegate protocol, for providing promised file data.

## See Also

### Initializers

init()

Initializes a file promise provider.

