

- Core Image
- CIDataMatrixCodeDescriptor
-  rowCount 

Instance Property

# rowCount

The number of module rows.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var rowCount: Int { get }
```

## Discussion

Refer to ISO/IEC 16022:2006(E) for valid module row and column count combinations.

## See Also

### Examining a Descriptor

var errorCorrectedPayload: Data

The error-corrected payload that comprises the Data Matrix code symbol.

var columnCount: Int

The number of module columns.

var eccVersion: CIDataMatrixCodeDescriptor.ECCVersion

The Data Matrix code ECC version.

