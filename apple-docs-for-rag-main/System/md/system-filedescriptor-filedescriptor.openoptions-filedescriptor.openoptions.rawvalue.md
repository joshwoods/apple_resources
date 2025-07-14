

- System
- FileDescriptor
- FileDescriptor.OpenOptions
-  FileDescriptor.OpenOptions.RawValue 

Type Alias

# FileDescriptor.OpenOptions.RawValue

The raw type that can be used to represent all values of the conforming type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
typealias RawValue = CInt
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

## See Also

### Interacting with C APIs

init(rawValue: CInt)

Create a strongly-typed options value from raw C options.

var rawValue: CInt

The raw C options.

