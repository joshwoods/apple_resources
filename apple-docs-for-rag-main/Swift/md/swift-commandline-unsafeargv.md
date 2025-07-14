

- Swift
- CommandLine
-  unsafeArgv 

Type Property

# unsafeArgv

Access to the raw argv value from C.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var unsafeArgv: UnsafeMutablePointer?> { get }
```

## Discussion

The value of this property is a `nil`-terminated C array. Including the trailing `nil`, there are argc `+ 1` elements in the array.

Note

Accessing the argument vector through this pointer is unsafe. Where possible, use arguments instead.

## See Also

### Accessing Raw Argument Data

static var argc: Int32

Access to the raw argc value from C.

