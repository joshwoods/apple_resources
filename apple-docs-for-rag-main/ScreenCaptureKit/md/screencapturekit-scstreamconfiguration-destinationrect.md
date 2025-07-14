

- ScreenCaptureKit
- SCStreamConfiguration
-  destinationRect 

Instance Property

# destinationRect

A rectangle that specifies a destination into which to write the output.

Mac Catalyst 18.2+macOS 12.3+

``` source
var destinationRect: CGRect { get set }
```

## Discussion

If you don’t specify a destination rectangle, the system uses the full dimensions of the output surface.

Note

The system doesn’t reference this value when capturing a single window because it draws the window into the output’s full bounds.

## See Also

### Specifying dimensions

var width: Int

The width of the output.

var height: Int

The height of the output.

var scalesToFit: Bool

A Boolean value that indicates whether to scale the output to fit the configured width and height.

var sourceRect: CGRect

A rectangle that specifies the source area to capture.

var preservesAspectRatio: Bool

A Boolean value that determines if the stream preserves aspect ratio.

