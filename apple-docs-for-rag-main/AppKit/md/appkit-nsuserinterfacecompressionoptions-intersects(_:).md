

- AppKit
- NSUserInterfaceCompressionOptions
-  intersects(\_:) 

Instance Method

# intersects(\_:)

Determines whether the supplied compression options intersect with the current instance’s options.

macOS 10.13+

``` source
func intersects(_ options: NSUserInterfaceCompressionOptions) -> Bool
```

## Parameters 

`options`  

A compression options object to compare with the current instance.

## Return Value

Returns true if at least one of the supplied options is present in the instance’s options, or false otherwise.

## See Also

### Comparing compression options

var isEmpty: Bool

A Boolean value that denotes whether the option is empty.

func contains(NSUserInterfaceCompressionOptions) -> Bool

Determines whether the supplied compression options are all present in the current instance.

