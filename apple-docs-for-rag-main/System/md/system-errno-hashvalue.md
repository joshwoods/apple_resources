

- System
- Errno
-  hashValue 

Instance Property

# hashValue

SystemSwiftiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var hashValue: Int { get }
```

Available when `Self` conforms to `Hashable` and `RawValue` conforms to `Hashable`.

## See Also

### Comparing Errors

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func ~= (Errno, any Error) -> Bool

func hash(into: inout Hasher)

