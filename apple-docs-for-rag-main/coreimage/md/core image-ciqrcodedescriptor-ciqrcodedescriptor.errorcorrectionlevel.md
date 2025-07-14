

- Core Image
- CIQRCodeDescriptor
-  CIQRCodeDescriptor.ErrorCorrectionLevel 

Enumeration

# CIQRCodeDescriptor.ErrorCorrectionLevel

Constants that indicate the percentage of the symbol dedicated to error correction.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
enum ErrorCorrectionLevel : Int, @unchecked Sendable
```

## Topics

### Enumeration Cases

case levelL

Low-percentage error correction: 20% of the symbol data is dedicated to error correction.

case levelM

Medium-percentage error correction: 37% of the symbol data is dedicated to error correction.

case levelQ

High-percentage error correction: 55% of the symbol data is dedicated to error correction.

case levelH

Very-high-percentage error correction: 65% of the symbol data is dedicated to error correction.

## Relationships

### Conforms To

- Sendable

