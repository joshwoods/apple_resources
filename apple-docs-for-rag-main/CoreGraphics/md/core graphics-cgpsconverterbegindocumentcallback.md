

- Core Graphics
-  CGPSConverterBeginDocumentCallback 

Type Alias

# CGPSConverterBeginDocumentCallback

Performs custom tasks at the beginning of a PostScript conversion process.

Mac CatalystmacOS

``` source
typealias CGPSConverterBeginDocumentCallback = (UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`info`  

A generic pointer to private data shared among your callback functions. This is the same pointer you supplied to init(info:callbacks:options:).

