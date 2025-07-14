

- ScreenCaptureKit
- SCStreamConfiguration
-  ignoreShadowsDisplay 

Instance Property

# ignoreShadowsDisplay

A Boolean value that indicates if the stream ignores the capturing of window shadows when streaming in display style.

Mac Catalyst 17.0+macOS 14.0+

``` source
var ignoreShadowsDisplay: Bool { get set }
```

## See Also

### Configuring captured elements

var showsCursor: Bool

A Boolean value that determines whether the cursor is visible in the stream.

var shouldBeOpaque: Bool

A Boolean value that indicates if semitransparent content presents as opaque.

var capturesShadowsOnly: Bool

A Boolean value that indicates if the stream only captures shadows.

var ignoreShadowsSingleWindow: Bool

A Boolean value that indicates if the stream ignores the capturing of window shadows when streaming in window style.

var ignoreGlobalClipDisplay: Bool

A Boolean value that indicates if the stream ignores content clipped past the edge of a display, when streaming in display style.

var ignoreGlobalClipSingleWindow: Bool

A Boolean value that indicates if the stream ignores content clipped past the edge of a display, when streaming in window style.

