

- MediaExtension
- MERAWProcessingParameter
-  enabled 

Instance Property

# enabled

A Boolean value that indicates whether the extension enables the parameter.

macOS 15.0+

``` source
var enabled: Bool { get set }
```

## Discussion

This parameter can only be modified by the extension. From the application-facing interface, `VTRAWProcessingSession`, this is a read-only value which indicates whether the parameter should be grayed out and disabled in any UI being generated.

## See Also

### Inspecting a processing parameter

var key: String

A unique key string identifying the parameter.

var longDescription: String

A localized description of the parameter, suitable for displaying in a tool tip or similar explanatory UI.

var name: String

A localized human-readable name for the parameter, suitable for displaying in application UI.

