

- Core NFC
- NFCTagReaderSession
- NFCTagReaderSession.PollingOption
-  iso14443 

Type Property

# iso14443

The option for detecting ISO 7816-compatible and MIFARE tags.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
static var iso14443: NFCTagReaderSession.PollingOption { get }
```

## Discussion

Supports NFC type A and B modulation.

## See Also

### Polling Options

static var iso15693: NFCTagReaderSession.PollingOption

The option for detecting ISO 15693 tags.

static var iso18092: NFCTagReaderSession.PollingOption

The option for detecting FeliCa tags.

