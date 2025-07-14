

- AppKit
- NSUserInterfaceCompressionOptions
-  contains(\_:) 

Instance Method

# contains(\_:)

Determines whether the supplied compression options are all present in the current instance.

macOS 10.13+

``` source
func contains(_ options: NSUserInterfaceCompressionOptions) -> Bool
```

## Parameters 

`options`  

A compression options object to compare with the current instance.

## Return Value

Returns true if all the supplied options are present in the instance’s options, or false otherwise.

## See Also

### Comparing compression options

var isEmpty: Bool

A Boolean value that denotes whether the option is empty.

func intersects(NSUserInterfaceCompressionOptions) -> Bool

Determines whether the supplied compression options intersect with the current instance’s options.

