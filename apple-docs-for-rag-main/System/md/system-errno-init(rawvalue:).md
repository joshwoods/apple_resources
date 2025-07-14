

- System
- Errno
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a strongly typed error number from a raw C error number.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(rawValue: CInt)
```

## See Also

### Interacting with C APIs

let rawValue: CInt

The raw C error number.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

