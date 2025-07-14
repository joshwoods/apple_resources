

- ScreenCaptureKit
- SCStreamConfiguration
-  shouldBeOpaque 

Instance Property

# shouldBeOpaque

A Boolean value that indicates if semitransparent content presents as opaque.

Mac Catalyst 17.0+macOS 14.0+

``` source
var shouldBeOpaque: Bool { get set }
```

## Discussion

When this property is `true`, semitransparent content in the stream presents as backed by a solid white background, making the resulting image fully opaque. The default value is `false`.

## See Also

### Configuring captured elements

var showsCursor: Bool

A Boolean value that determines whether the cursor is visible in the stream.

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

