

- AppKit
- NSUserInterfaceCompressionOptions
-  breakEqualWidths 

Type Property

# breakEqualWidths

An option specifying that views should no longer maintain equal width constraints.

macOS 10.13+

``` source
@NSCopying
class var breakEqualWidths: NSUserInterfaceCompressionOptions { get }
```

## Discussion

This option is handled by the system, and no action is required by the views.

## See Also

### Creating standard options

class var hideImages: NSUserInterfaceCompressionOptions

An option specifying that views should hide their images.

class var hideText: NSUserInterfaceCompressionOptions

An option specifying that views should hide their text.

class var reduceMetrics: NSUserInterfaceCompressionOptions

An option specifying that views should reduce their internal metrics.

class var standardOptions: NSUserInterfaceCompressionOptions

An option that represents the union of all standard compression options.

