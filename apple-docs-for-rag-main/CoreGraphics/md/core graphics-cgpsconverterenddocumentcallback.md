

- Core Graphics
-  CGPSConverterEndDocumentCallback 

Type Alias

# CGPSConverterEndDocumentCallback

Performs custom tasks at the end of a PostScript conversion process.

Mac CatalystmacOS

``` source
typealias CGPSConverterEndDocumentCallback = (UnsafeMutableRawPointer?, Bool) -> Void
```

## Parameters 

`info`  

A generic pointer to private data shared among your callback functions. This is the same pointer you supplied to init(info:callbacks:options:).

`success`  

A Boolean value that indicates whether the PostScript conversion completed successfully (true if it did).

