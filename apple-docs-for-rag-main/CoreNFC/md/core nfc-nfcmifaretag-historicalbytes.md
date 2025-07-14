

- Core NFC
- NFCMiFareTag
-  historicalBytes 

Instance Property

# historicalBytes

The historical bytes extracted from an Answer To Select response.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var historicalBytes: Data? { get }
```

**Required**

## See Also

### Getting Tag Information

var mifareFamily: NFCMiFareFamily

The MIFARE product family identifier for the tag.

**Required**

enum NFCMiFareFamily

Identifiers for the MIFARE product families.

var identifier: Data

The unique hardware identifier of the tag.

**Required**

