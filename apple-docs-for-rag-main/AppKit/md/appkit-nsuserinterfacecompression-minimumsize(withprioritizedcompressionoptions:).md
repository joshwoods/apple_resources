

- AppKit
- NSUserInterfaceCompression
-  minimumSize(withPrioritizedCompressionOptions:) 

Instance Method

# minimumSize(withPrioritizedCompressionOptions:)

Returns the minimum size a view can achieve by applying the supplied compression options.

macOS 10.13+

``` source
func minimumSize(withPrioritizedCompressionOptions prioritizedOptions: [NSUserInterfaceCompressionOptions]) -> NSSize
```

**Required**

## Parameters 

`prioritizedOptions`  

An array of compression options that the view should apply to reduce its size.

## Return Value

The minimum size of a view when applying the supplied compression options.

## Discussion

Compression options that are handled by the system are not included in the supplied array.

## See Also

### Querying Compression Status

var activeCompressionOptions: NSUserInterfaceCompressionOptions

The compression options that are currently applied to the view.

**Required**

