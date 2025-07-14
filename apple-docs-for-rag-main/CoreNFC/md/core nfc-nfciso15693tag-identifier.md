

- Core NFC
- NFCISO15693Tag
-  identifier 

Instance Property

# identifier

The unique hardware identifier of the tag.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var identifier: Data { get }
```

**Required**

## Discussion

The identifier data is in big-endian byte order.

## See Also

### Getting Tag Information

var icManufacturerCode: Int

The IC manufacturer code of the tag.

**Required**

var icSerialNumber: Data

The IC serial number assigned to the tag by the manufacturer.

**Required**

