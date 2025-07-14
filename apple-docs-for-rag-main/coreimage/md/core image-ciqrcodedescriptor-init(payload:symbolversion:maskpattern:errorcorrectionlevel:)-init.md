

- Core Image
- CIQRCodeDescriptor
-  init(payload:symbolVersion:maskPattern:errorCorrectionLevel:) 

Initializer

# init(payload:symbolVersion:maskPattern:errorCorrectionLevel:)

Initializes a descriptor that can be used as input to the `CIBarcodeGenerator` filter.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init?(
    payload errorCorrectedPayload: Data,
    symbolVersion: Int,
    maskPattern: UInt8,
    errorCorrectionLevel: CIQRCodeDescriptor.ErrorCorrectionLevel
)
```

## Parameters 

`errorCorrectedPayload`  

The data to encode in the QR code.

`symbolVersion`  

The symbol version, from 1 through 40.

`maskPattern`  

The mask pattern to use in the QR code.

`errorCorrectionLevel`  

The QR code's error correction level: `L`, `M`, `Q`, or `H`.

## Return Value

A QR code descriptor encoding the specified data at the specified error correction level.

## Discussion

The `CIBarcodeGenerator` filter can recreate a QR code given the descriptor created using this method.

