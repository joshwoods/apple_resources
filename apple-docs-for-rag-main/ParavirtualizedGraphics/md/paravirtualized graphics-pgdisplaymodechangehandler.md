

- Paravirtualized Graphics
-  PGDisplayModeChangeHandler 

Type Alias

# PGDisplayModeChangeHandler

The block signature for a routine that handles changes to the display’s graphics mode.

Mac Catalyst 14.0+macOS 11.0+

``` source
typealias PGDisplayModeChangeHandler = (PGDisplayCoord_t, OSType) -> Void
```

## Parameters 

`sizeInPixels`  

The dimensions of the new display mode.

`pixelFormat`  

The pixel format of the new display mode.

## See Also

### Handling Mode Changes

var modeChangeHandler: PGDisplayModeChangeHandler?

A handler that the framework calls to change the virtual display’s graphics mode.

