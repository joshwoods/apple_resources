

- ScreenCaptureKit
- SCStreamConfiguration
-  ignoreGlobalClipSingleWindow 

Instance Property

# ignoreGlobalClipSingleWindow

A Boolean value that indicates if the stream ignores content clipped past the edge of a display, when streaming in window style.

Mac Catalyst 17.0+macOS 14.0+

``` source
var ignoreGlobalClipSingleWindow: Bool { get set }
```

## Discussion

The display that originates the stream determines clipping bounds. When this value is `true`, the stream contains content moved past the clipping bounds. The default value is `false`.

## See Also

### Configuring captured elements

var showsCursor: Bool

A Boolean value that determines whether the cursor is visible in the stream.

var shouldBeOpaque: Bool

A Boolean value that indicates if semitransparent content presents as opaque.

var capturesShadowsOnly: Bool

A Boolean value that indicates if the stream only captures shadows.

var ignoreShadowsDisplay: Bool

A Boolean value that indicates if the stream ignores the capturing of window shadows when streaming in display style.

var ignoreShadowsSingleWindow: Bool

A Boolean value that indicates if the stream ignores the capturing of window shadows when streaming in window style.

var ignoreGlobalClipDisplay: Bool

A Boolean value that indicates if the stream ignores content clipped past the edge of a display, when streaming in display style.

