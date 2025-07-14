

- AppKit
- NSUserInterfaceCompressionOptions
-  reduceMetrics 

Type Property

# reduceMetrics

An option specifying that views should reduce their internal metrics.

macOS 10.13+

``` source
@NSCopying
class var reduceMetrics: NSUserInterfaceCompressionOptions { get }
```

## Discussion

Use this compression option to reduce the padding in system controls.

## See Also

### Creating standard options

class var hideImages: NSUserInterfaceCompressionOptions

An option specifying that views should hide their images.

class var hideText: NSUserInterfaceCompressionOptions

An option specifying that views should hide their text.

class var breakEqualWidths: NSUserInterfaceCompressionOptions

An option specifying that views should no longer maintain equal width constraints.

class var standardOptions: NSUserInterfaceCompressionOptions

An option that represents the union of all standard compression options.

