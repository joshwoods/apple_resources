

- Core Image
- CIAztecCodeDescriptor
-  init(payload:isCompact:layerCount:dataCodewordCount:) 

Initializer

# init(payload:isCompact:layerCount:dataCodewordCount:)

Initializes a descriptor that can be used as input to the `CIBarcodeGenerator` filter.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init?(
    payload errorCorrectedPayload: Data,
    isCompact: Bool,
    layerCount: Int,
    dataCodewordCount: Int
)
```

## Parameters 

`errorCorrectedPayload`  

The data to encode in the Aztec code.

`isCompact`  

A Boolean indicating whether or not the Aztec code is compact.

`layerCount`  

The number of layers in the Aztec code.

`dataCodewordCount`  

The number of codewords in the Aztec code.

## Return Value

An Aztec code descriptor encoding the specified payload with the specified number of layers and data codewords.

## Discussion

The `CIBarcodeGenerator` filter can recreate an Aztec code given the descriptor created using this method.

