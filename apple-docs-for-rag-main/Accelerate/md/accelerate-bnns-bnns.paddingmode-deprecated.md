

- Accelerate
- BNNS
-  BNNS.PaddingMode Deprecated

Enumeration

# BNNS.PaddingMode

Constants that define padding modes.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOSwatchOS 7.0+tvOS 14.0+

``` source
enum PaddingMode
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Enumeration Cases

case constantBitPattern(UInt32)

A constant that indicates that a padding operation fills the padded area with a specified bit pattern.

case constantScalar(Float)

A constant that indicates that a padding operation fills the padded area with a specified scalar value.

case reflect

A constant that indicates that a padding operation fills the padded area to form an odd-symmetric pattern.

case symmetric

A constant that indicates that a padding operation fills the padded area to form an even-symmetric pattern.

### Instance Properties

var bnnsPaddingMode: BNNSPaddingMode

The underlying padding mode structure.

var paddingBitPattern: UInt32

The padding bit pattern.

