

- AppKit
- NSImage
-  delegate 

Instance Property

# delegate

The image’s delegate object.

macOS

``` source
weak var delegate: (any NSImageDelegate)? { get set }
```

## Discussion

By default, this property contains `nil`.

## See Also

### Managing Loading and Drawing of Images

protocol NSImageDelegate

A set of optional methods that you can use to respond to drawing failures and manage incremental loads.

