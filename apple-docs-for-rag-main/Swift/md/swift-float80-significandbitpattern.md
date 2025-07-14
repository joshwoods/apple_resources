

- Swift
- Float80
-  significandBitPattern 

Instance Property

# significandBitPattern

The raw encoding of the value’s significand field.

macOS 10.10+

``` source
var significandBitPattern: UInt64 { get }
```

## Discussion

The `significandBitPattern` property does not include the leading integral bit of the significand, even for types like `Float80` that store it explicitly.

