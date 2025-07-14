

- Core Image
- CIDataMatrixCodeDescriptor
-  eccVersion 

Instance Property

# eccVersion

The Data Matrix code ECC version.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var eccVersion: CIDataMatrixCodeDescriptor.ECCVersion { get }
```

## Discussion

Valid values are 000, 050, 080, 100, 140, and 200. Any symbol with an even number of rows and columns will be ECC 200.

## See Also

### Examining a Descriptor

var errorCorrectedPayload: Data

The error-corrected payload that comprises the Data Matrix code symbol.

var rowCount: Int

The number of module rows.

var columnCount: Int

The number of module columns.

