

- AppKit
- NSGroupTouchBarItem
-  prioritizedCompressionOptions 

Instance Property

# prioritizedCompressionOptions

The allowed compression options, in the order they should be applied.

macOS 10.13+

``` source
@MainActor
var prioritizedCompressionOptions: [NSUserInterfaceCompressionOptions] { get set }
```

## Discussion

Use this property when you want to control the order of the system compression options, or if you want to use custom compression options.

The default value is an array containing all standard AppKit options, in the AppKit-defined order.

## See Also

### Configuring item compression

var effectiveCompressionOptions: NSUserInterfaceCompressionOptions

The compression options that are currently active on the group.

