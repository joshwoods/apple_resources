

- Accelerate
- BNNS
-  BNNS.RandomGeneratorMethod 

Enumeration

# BNNS.RandomGeneratorMethod

Constants that describe random number generation methods.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
enum RandomGeneratorMethod
```

## Topics

### Random Number Generation Methods

case aesCtr

A constant that specifes an implementation that’s based on the Advanced Encryption Standard (AES) hash of a counter.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Creating a Random Number Generator

init?(method: BNNS.RandomGeneratorMethod, seed: UInt64?, filterParameters: BNNSFilterParameters?)

Returns a new random number generator.

