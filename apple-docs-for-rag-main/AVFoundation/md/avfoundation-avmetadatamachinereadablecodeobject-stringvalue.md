

- AVFoundation
- AVMetadataMachineReadableCodeObject
-  stringValue 

Instance Property

# stringValue

Returns the error-corrected data decoded into a human-readable string.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.15+tvOS 9.0+

``` source
var stringValue: String? { get }
```

## Discussion

The value of this property is an `NSString` created by decoding the binary payload according to the format of the machine-readable code, or `nil` if a string representation cannot be created.

## See Also

### Getting Machine Readable Code Values

var corners: [CGPoint]

A Swift array of corner points.

var descriptor: CIBarcodeDescriptor?

A barcode description for use in Core Image.

