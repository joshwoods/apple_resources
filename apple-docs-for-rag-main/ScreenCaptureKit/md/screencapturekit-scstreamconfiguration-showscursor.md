

- ScreenCaptureKit
- SCStreamConfiguration
-  showsCursor 

Instance Property

# showsCursor

A Boolean value that determines whether the cursor is visible in the stream.

Mac Catalyst 18.2+macOS 12.3+

``` source
var showsCursor: Bool { get set }
```

## Discussion

The cursor is visible by default.

## See Also

### Configuring captured elements

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

var ignoreGlobalClipSingleWindow: Bool

A Boolean value that indicates if the stream ignores content clipped past the edge of a display, when streaming in window style.

