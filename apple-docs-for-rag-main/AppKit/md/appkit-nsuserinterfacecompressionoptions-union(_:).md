

- AppKit
- NSUserInterfaceCompressionOptions
-  union(\_:) 

Instance Method

# union(\_:)

Creates a new compression options object representing the union with the provided options.

macOS 10.13+

``` source
func union(_ options: NSUserInterfaceCompressionOptions) -> NSUserInterfaceCompressionOptions
```

## Parameters 

`options`  

A set of compression options to add to the current object.

## Return Value

A new `NSCompressibleUserInterfaceOptions` object which represents the union with the supplied compression options.

## See Also

### Combining compression options

func subtracting(NSUserInterfaceCompressionOptions) -> NSUserInterfaceCompressionOptions

Creates a new compression options object with the supplied options removed.

