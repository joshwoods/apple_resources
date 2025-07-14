

- Core Graphics
-  CGPSConverterReleaseInfoCallback 

Type Alias

# CGPSConverterReleaseInfoCallback

Performs custom tasks when a PostScript converter is released.

Mac CatalystmacOS

``` source
typealias CGPSConverterReleaseInfoCallback = (UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`info`  

A generic pointer to private data shared among your callback functions. This is the same pointer you supplied to init(info:callbacks:options:).

