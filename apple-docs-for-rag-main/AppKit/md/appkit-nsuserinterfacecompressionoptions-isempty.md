

- AppKit
- NSUserInterfaceCompressionOptions
-  isEmpty 

Instance Property

# isEmpty

A Boolean value that denotes whether the option is empty.

macOS 10.13+

``` source
var isEmpty: Bool { get }
```

## Discussion

Returns true if the option is equivalent to the empty set, or false otherwise.

## See Also

### Comparing compression options

func contains(NSUserInterfaceCompressionOptions) -> Bool

Determines whether the supplied compression options are all present in the current instance.

func intersects(NSUserInterfaceCompressionOptions) -> Bool

Determines whether the supplied compression options intersect with the current instance’s options.

