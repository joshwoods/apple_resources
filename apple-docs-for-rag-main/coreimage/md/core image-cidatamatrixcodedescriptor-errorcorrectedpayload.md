

- Core Image
- CIDataMatrixCodeDescriptor
-  errorCorrectedPayload 

Instance Property

# errorCorrectedPayload

The error-corrected payload that comprises the Data Matrix code symbol.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var errorCorrectedPayload: Data { get }
```

## Discussion

The error-corrected payload contains the de-interleaved bits of the message.

Data Matrix symbols are specified by ISO/IEC 16022:2006(E). ECC 200-type symbols will always have an even number of rows and columns.

## See Also

### Examining a Descriptor

var rowCount: Int

The number of module rows.

var columnCount: Int

The number of module columns.

var eccVersion: CIDataMatrixCodeDescriptor.ECCVersion

The Data Matrix code ECC version.

