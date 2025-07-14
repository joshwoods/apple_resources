

- ScreenCaptureKit
- SCStreamConfiguration
-  sourceRect 

Instance Property

# sourceRect

A rectangle that specifies the source area to capture.

Mac Catalyst 18.2+macOS 12.3+

``` source
var sourceRect: CGRect { get set }
```

## Discussion

If you don’t specify a source rectangle to capture, the system captures the entire display.

Note

The system doesn’t reference this value when you capture a single window because it captures the full bounds of the window.

## See Also

### Specifying dimensions

var width: Int

The width of the output.

var height: Int

The height of the output.

var scalesToFit: Bool

A Boolean value that indicates whether to scale the output to fit the configured width and height.

var destinationRect: CGRect

A rectangle that specifies a destination into which to write the output.

var preservesAspectRatio: Bool

A Boolean value that determines if the stream preserves aspect ratio.

