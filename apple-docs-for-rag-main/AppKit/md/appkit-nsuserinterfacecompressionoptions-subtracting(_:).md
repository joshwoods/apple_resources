

- AppKit
- NSUserInterfaceCompressionOptions
-  subtracting(\_:) 

Instance Method

# subtracting(\_:)

Creates a new compression options object with the supplied options removed.

macOS 10.13+

``` source
func subtracting(_ options: NSUserInterfaceCompressionOptions) -> NSUserInterfaceCompressionOptions
```

## Parameters 

`options`  

A set of compression options to remove from the current object.

## Return Value

A new `NSCompressibleUserInterfaceOptions` object with the supplied options removed.

## See Also

### Combining compression options

func union(NSUserInterfaceCompressionOptions) -> NSUserInterfaceCompressionOptions

Creates a new compression options object representing the union with the provided options.

