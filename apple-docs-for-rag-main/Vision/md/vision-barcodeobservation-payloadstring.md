

- Vision
- BarcodeObservation
-  payloadString 

Instance Property

# payloadString

A string value that represents the barcode payload.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let payloadString: String?
```

## Discussion

Depending on the symbology or the payload data itself, a string representation of the payload may not be available.

## See Also

### Getting the payload

let payloadData: Data?

The raw data representation of the barcode’s payload.

let supplementalPayloadData: Data?

The raw data representation of the barcode’s supplemental payload.

let supplementalPayloadString: String?

The supplemental code decoded as a string value.

