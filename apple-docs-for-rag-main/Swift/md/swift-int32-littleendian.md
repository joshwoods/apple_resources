

- Swift
- Int32
-  littleEndian 

Instance Property

# littleEndian

The little-endian representation of this integer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var littleEndian: Self { get }
```

## Discussion

If necessary, the byte order of this value is reversed from the typical byte order of this integer type. On a little-endian platform, for any integer `x`, `x == x.littleEndian`.

