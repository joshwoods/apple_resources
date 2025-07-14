

- Swift
- Float16
-  significandBitPattern 

Instance Property

# significandBitPattern

The raw encoding of the value’s significand field.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var significandBitPattern: UInt16 { get }
```

## Discussion

The `significandBitPattern` property does not include the leading integral bit of the significand, even for types like `Float80` that store it explicitly.

