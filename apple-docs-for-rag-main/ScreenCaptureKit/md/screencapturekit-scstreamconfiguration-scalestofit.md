

- ScreenCaptureKit
- SCStreamConfiguration
-  scalesToFit 

Instance Property

# scalesToFit

A Boolean value that indicates whether to scale the output to fit the configured width and height.

Mac Catalyst 18.2+macOS 12.3+

``` source
var scalesToFit: Bool { get set }
```

## Discussion

The system uses this value during independent window capture.

## See Also

### Specifying dimensions

var width: Int

The width of the output.

var height: Int

The height of the output.

var sourceRect: CGRect

A rectangle that specifies the source area to capture.

var destinationRect: CGRect

A rectangle that specifies a destination into which to write the output.

var preservesAspectRatio: Bool

A Boolean value that determines if the stream preserves aspect ratio.

