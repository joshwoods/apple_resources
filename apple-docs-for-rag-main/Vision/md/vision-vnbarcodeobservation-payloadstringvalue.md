

- Vision
- VNBarcodeObservation
-  payloadStringValue 

Instance Property

# payloadStringValue

A string value that represents the barcode payload.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var payloadStringValue: String? { get }
```

## Discussion

Depending on the symbology or the payload data itself, a string representation of the payload may not be available.

## See Also

### Parsing the Payload

var payloadData: Data?

The raw data representation of the barcode’s payload.

var supplementalPayloadString: String?

The supplemental code decoded as a string value.

var supplementalPayloadData: Data?

var supplementalCompositeType: VNBarcodeCompositeType

The supplemental composite type.

var isGS1DataCarrier: Bool

A Boolean value that indicates whether the barcode carries any global standards data.

