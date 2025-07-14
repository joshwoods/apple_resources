

- AppKit
- NSButton
-  compress(withPrioritizedCompressionOptions:) 

Instance Method

# compress(withPrioritizedCompressionOptions:)

Sets the priority compression options for this button.

macOS 10.13+

``` source
@MainActor
func compress(withPrioritizedCompressionOptions prioritizedOptions: [NSUserInterfaceCompressionOptions])
```

## Parameters 

`prioritizedOptions`  

An array of interface compression options.

## See Also

### Managing Button Compression

var activeCompressionOptions: NSUserInterfaceCompressionOptions

The compression options active for this button.

func minimumSize(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions]) -> NSSize

Returns the minimum size of the button by using the compression options.

