

- Core NFC
- NFCMiFareTag
-  mifareFamily 

Instance Property

# mifareFamily

The MIFARE product family identifier for the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var mifareFamily: NFCMiFareFamily { get }
```

**Required**

## See Also

### Getting Tag Information

enum NFCMiFareFamily

Identifiers for the MIFARE product families.

var identifier: Data

The unique hardware identifier of the tag.

**Required**

var historicalBytes: Data?

The historical bytes extracted from an Answer To Select response.

**Required**

