

- Swift
- Float16
-  init(bitPattern:) 

Initializer

# init(bitPattern:)

Creates a new value with the given bit pattern.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(bitPattern: UInt16)
```

## Parameters 

`bitPattern`  

The integer encoding of a `Float16` instance.

## Discussion

The value passed as `bitPattern` is interpreted in the binary interchange format defined by the IEEE 754 specification.

