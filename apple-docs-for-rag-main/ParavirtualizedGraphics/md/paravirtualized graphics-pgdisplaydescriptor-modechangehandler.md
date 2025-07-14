

- Paravirtualized Graphics
- PGDisplayDescriptor
-  modeChangeHandler 

Instance Property

# modeChangeHandler

A handler that the framework calls to change the virtual display’s graphics mode.

Mac Catalyst 14.0+macOS 11.0+

``` source
var modeChangeHandler: PGDisplayModeChangeHandler? { get set }
```

## See Also

### Handling Mode Changes

typealias PGDisplayModeChangeHandler

The block signature for a routine that handles changes to the display’s graphics mode.

