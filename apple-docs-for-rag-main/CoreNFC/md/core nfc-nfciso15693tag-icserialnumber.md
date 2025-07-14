

- Core NFC
- NFCISO15693Tag
-  icSerialNumber 

Instance Property

# icSerialNumber

The IC serial number assigned to the tag by the manufacturer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var icSerialNumber: Data { get }
```

**Required**

## Discussion

The IC serial number comes from bits 1 through 48 of the identifier data and is in big-endian byte order.

## See Also

### Getting Tag Information

var icManufacturerCode: Int

The IC manufacturer code of the tag.

**Required**

var identifier: Data

The unique hardware identifier of the tag.

**Required**

