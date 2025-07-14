

- System
- FileDescriptor
- FileDescriptor.OpenOptions
-  init(rawValue:) 

Initializer

# init(rawValue:)

Create a strongly-typed options value from raw C options.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(rawValue: CInt)
```

## See Also

### Interacting with C APIs

var rawValue: CInt

The raw C options.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

