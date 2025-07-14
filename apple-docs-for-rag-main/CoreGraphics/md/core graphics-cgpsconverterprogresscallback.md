

- Core Graphics
-  CGPSConverterProgressCallback 

Type Alias

# CGPSConverterProgressCallback

Reports progress periodically during a PostScript conversion process.

Mac CatalystmacOS

``` source
typealias CGPSConverterProgressCallback = (UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`info`  

A generic pointer to private data shared among your callback functions. This is the same pointer you supplied to init(info:callbacks:options:).

