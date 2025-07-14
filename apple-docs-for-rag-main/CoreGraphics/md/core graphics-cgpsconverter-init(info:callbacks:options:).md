

- Core Graphics
- CGPSConverter
-  init(info:callbacks:options:) 

Initializer

# init(info:callbacks:options:)

Creates a new PostScript converter.

Mac Catalyst 13.1+macOS 10.3+

``` source
init?(
    info: UnsafeMutableRawPointer?,
    callbacks: UnsafePointer,
    options: CFDictionary?
)
```

## Parameters 

`info`  

A pointer to the data that will be passed to the callbacks.

`callbacks`  

A pointer to a PostScript converter callbacks structure that specifies the callbacks to be used during a conversion process.

`options`  

This parameter should be `NULL`; it is reserved for future expansion of the API.

## Return Value

A new PostScript converter, or `NULL` if a converter could not be created. You are responsible for releasing this object.

