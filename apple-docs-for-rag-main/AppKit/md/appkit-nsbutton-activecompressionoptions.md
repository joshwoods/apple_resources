

- AppKit
- NSButton
-  activeCompressionOptions 

Instance Property

# activeCompressionOptions

The compression options active for this button.

macOS 10.13+

``` source
@NSCopying @MainActor
var activeCompressionOptions: NSUserInterfaceCompressionOptions { get }
```

## Discussion

Only compression options that have been applied and are actively being respected are returned. For more information about managing button sizes when space is restriced, see NSUserInterfaceCompressionOptions.

## See Also

### Managing Button Compression

func compress(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions])

Sets the priority compression options for this button.

func minimumSize(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions]) -> NSSize

Returns the minimum size of the button by using the compression options.

