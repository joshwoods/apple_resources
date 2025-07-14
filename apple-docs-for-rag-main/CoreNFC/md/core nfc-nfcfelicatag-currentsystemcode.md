

- Core NFC
- NFCFeliCaTag
-  currentSystemCode 

Instance Property

# currentSystemCode

The system code most recently selected by the reader session during a polling sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var currentSystemCode: Data { get }
```

**Required**

## Discussion

The system code matches one of the entries in the array for the com.apple.developer.nfc.readersession.felica.systemcodes information property list key.

## See Also

### Getting Current Information

var currentIDm: Data

The manufacturer identifier for the system currently selected by the reader session.

**Required**

