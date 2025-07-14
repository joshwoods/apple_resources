

- Foundation
- JSONDecoder
-  JSONDecoder.NonConformingFloatDecodingStrategy 

Enumeration

# JSONDecoder.NonConformingFloatDecodingStrategy

The strategies for encoding nonconforming floating-point numbers, also known as IEEE 754 exceptional values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum NonConformingFloatDecodingStrategy
```

## Overview

The IEEE 754 floating-point specification defines exceptional values, which include infinity and nan.

## Topics

### Exceptional Values

case convertFromString(positiveInfinity: String, negativeInfinity: String, nan: String)

The strategy that decodes exceptional floating-point values from a specified string representation.

case `throw`

The strategy that throws an error upon decoding an exceptional floating-point value.

## Relationships

### Conforms To

- Sendable

## See Also

### Decoding Exceptional Numbers

var nonConformingFloatDecodingStrategy: JSONDecoder.NonConformingFloatDecodingStrategy

The strategy used by a decoder when it encounters exceptional floating-point values.

