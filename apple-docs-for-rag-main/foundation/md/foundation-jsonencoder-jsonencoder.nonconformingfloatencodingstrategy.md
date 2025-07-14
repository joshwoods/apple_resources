

- Foundation
- JSONEncoder
-  JSONEncoder.NonConformingFloatEncodingStrategy 

Enumeration

# JSONEncoder.NonConformingFloatEncodingStrategy

The strategies for encoding nonconforming floating-point numbers, also known as IEEE 754 exceptional values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum NonConformingFloatEncodingStrategy
```

## Overview

The IEEE 754 floating-point specification defines exceptional values, which include infinity and nan.

## Topics

### Exceptional Values

case convertToString(positiveInfinity: String, negativeInfinity: String, nan: String)

The strategy that encodes exceptional floating-point values from a specified string representation.

case `throw`

The strategy that throws an error upon encoding an exceptional floating-point value.

## Relationships

### Conforms To

- Sendable

## See Also

### Encoding Exceptional Numbers

var nonConformingFloatEncodingStrategy: JSONEncoder.NonConformingFloatEncodingStrategy

The strategy used by an encoder when it encounters exceptional floating-point values.

