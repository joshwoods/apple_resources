

- AppKit
- NSUserInterfaceCompressionOptions
-  standardOptions 

Type Property

# standardOptions

An option that represents the union of all standard compression options.

macOS 10.13+

``` source
@NSCopying
class var standardOptions: NSUserInterfaceCompressionOptions { get }
```

## See Also

### Creating standard options

class var hideImages: NSUserInterfaceCompressionOptions

An option specifying that views should hide their images.

class var hideText: NSUserInterfaceCompressionOptions

An option specifying that views should hide their text.

class var reduceMetrics: NSUserInterfaceCompressionOptions

An option specifying that views should reduce their internal metrics.

class var breakEqualWidths: NSUserInterfaceCompressionOptions

An option specifying that views should no longer maintain equal width constraints.

