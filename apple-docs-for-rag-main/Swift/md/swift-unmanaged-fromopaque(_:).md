

- Swift
- Unmanaged
-  fromOpaque(\_:) 

Type Method

# fromOpaque(\_:)

Unsafely turns an opaque C pointer into an unmanaged class reference.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func fromOpaque(_ value: UnsafeRawPointer) -> Unmanaged
```

## Parameters 

`value`  

An opaque C pointer.

## Return Value

An unmanaged class reference to `value`.

## Discussion

This operation does not change reference counts.

```
let str: CFString = Unmanaged.fromOpaque(ptr).takeUnretainedValue()
```

