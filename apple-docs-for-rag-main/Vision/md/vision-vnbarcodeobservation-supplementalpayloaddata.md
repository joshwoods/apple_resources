

- Vision
- VNBarcodeObservation
-  supplementalPayloadData 

Instance Property

# supplementalPayloadData

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var supplementalPayloadData: Data? { get }
```

## See Also

### Parsing the Payload

var payloadStringValue: String?

A string value that represents the barcode payload.

var payloadData: Data?

The raw data representation of the barcode’s payload.

var supplementalPayloadString: String?

The supplemental code decoded as a string value.

var supplementalCompositeType: VNBarcodeCompositeType

The supplemental composite type.

var isGS1DataCarrier: Bool

A Boolean value that indicates whether the barcode carries any global standards data.

