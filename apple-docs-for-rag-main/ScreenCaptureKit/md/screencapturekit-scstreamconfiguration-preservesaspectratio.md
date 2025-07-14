

- ScreenCaptureKit
- SCStreamConfiguration
-  preservesAspectRatio 

Instance Property

# preservesAspectRatio

A Boolean value that determines if the stream preserves aspect ratio.

Mac Catalyst 17.0+macOS 14.0+

``` source
var preservesAspectRatio: Bool { get set }
```

## Discussion

The default value is `true`.

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

var destinationRect: CGRect

A rectangle that specifies a destination into which to write the output.

