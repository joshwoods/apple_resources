

- Swift
- Unmanaged
-  toOpaque() 

Instance Method

# toOpaque()

Unsafely converts an unmanaged class reference to a pointer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func toOpaque() -> UnsafeMutableRawPointer
```

## Return Value

An opaque pointer to the value of this unmanaged reference.

## Discussion

This operation does not change reference counts.

```
let str0 = "boxcar" as CFString
let bits = Unmanaged.passUnretained(str0)
let ptr = bits.toOpaque()
```

