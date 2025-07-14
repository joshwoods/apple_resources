

- Core NFC
- NFCMiFareTag
-  identifier 

Instance Property

# identifier

The unique hardware identifier of the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var identifier: Data { get }
```

**Required**

## Discussion

The identifier data is in big-endian byte order.

## See Also

### Getting Tag Information

var mifareFamily: NFCMiFareFamily

The MIFARE product family identifier for the tag.

**Required**

enum NFCMiFareFamily

Identifiers for the MIFARE product families.

var historicalBytes: Data?

The historical bytes extracted from an Answer To Select response.

**Required**

