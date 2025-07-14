

- AppKit
- NSUserInterfaceCompression
-  activeCompressionOptions 

Instance Property

# activeCompressionOptions

The compression options that are currently applied to the view.

macOS 10.13+

``` source
@NSCopying
var activeCompressionOptions: NSUserInterfaceCompressionOptions { get }
```

**Required**

## Discussion

This property includes only those compression options applied to the view that are actively being respected.

## See Also

### Querying Compression Status

func minimumSize(withPrioritizedCompressionOptions: [NSUserInterfaceCompressionOptions]) -> NSSize

Returns the minimum size a view can achieve by applying the supplied compression options.

**Required**

