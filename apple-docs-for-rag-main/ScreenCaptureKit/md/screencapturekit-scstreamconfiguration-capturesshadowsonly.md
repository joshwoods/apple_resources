

- ScreenCaptureKit
- SCStreamConfiguration
-  capturesShadowsOnly 

Instance Property

# capturesShadowsOnly

A Boolean value that indicates if the stream only captures shadows.

Mac Catalyst 17.0+macOS 14.0+

``` source
var capturesShadowsOnly: Bool { get set }
```

## Discussion

The default value is `false`.

## See Also

### Configuring captured elements

var showsCursor: Bool

A Boolean value that determines whether the cursor is visible in the stream.

var shouldBeOpaque: Bool

A Boolean value that indicates if semitransparent content presents as opaque.

var ignoreShadowsDisplay: Bool

A Boolean value that indicates if the stream ignores the capturing of window shadows when streaming in display style.

var ignoreShadowsSingleWindow: Bool

A Boolean value that indicates if the stream ignores the capturing of window shadows when streaming in window style.

var ignoreGlobalClipDisplay: Bool

A Boolean value that indicates if the stream ignores content clipped past the edge of a display, when streaming in display style.

var ignoreGlobalClipSingleWindow: Bool

A Boolean value that indicates if the stream ignores content clipped past the edge of a display, when streaming in window style.

