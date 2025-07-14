

- AppKit
- NSButton
-  minimumSize(withPrioritizedCompressionOptions:) 

Instance Method

# minimumSize(withPrioritizedCompressionOptions:)

Returns the minimum size of the button by using the compression options.

macOS 10.13+

``` source
@MainActor
func minimumSize(withPrioritizedCompressionOptions prioritizedOptions: [NSUserInterfaceCompressionOptions]) -> NSSize
```

## Parameters 

`prioritizedOptions`  

An array of interface compression options.

## Return Value

The size of the compressed button.

## See Also

### Managing Button Compression

var activeCompressionOptions: NSUserInterfaceCompressionOptions

The compression options active for this button.

func compress(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions])

Sets the priority compression options for this button.

