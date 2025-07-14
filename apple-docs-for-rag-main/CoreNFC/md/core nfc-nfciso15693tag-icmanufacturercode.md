

- Core NFC
- NFCISO15693Tag
-  icManufacturerCode 

Instance Property

# icManufacturerCode

The IC manufacturer code of the tag.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var icManufacturerCode: Int { get }
```

**Required**

## Discussion

The IC manufacturer code comes from bits 49 through 56 of the identifier data, in accordance with ISO/IEC 7816-6:2004.

## See Also

### Getting Tag Information

var icSerialNumber: Data

The IC serial number assigned to the tag by the manufacturer.

**Required**

var identifier: Data

The unique hardware identifier of the tag.

**Required**

