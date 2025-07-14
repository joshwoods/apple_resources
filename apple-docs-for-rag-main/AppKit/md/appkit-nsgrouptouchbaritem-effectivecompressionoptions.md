

- AppKit
- NSGroupTouchBarItem
-  effectiveCompressionOptions 

Instance Property

# effectiveCompressionOptions

The compression options that are currently active on the group.

macOS 10.13+

``` source
@MainActor
var effectiveCompressionOptions: NSUserInterfaceCompressionOptions { get }
```

## See Also

### Configuring item compression

var prioritizedCompressionOptions: [NSUserInterfaceCompressionOptions]

The allowed compression options, in the order they should be applied.

