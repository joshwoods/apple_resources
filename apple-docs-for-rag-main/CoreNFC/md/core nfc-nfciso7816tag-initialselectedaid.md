

- Core NFC
- NFCISO7816Tag
-  initialSelectedAID 

Instance Property

# initialSelectedAID

A hexadecimal string of the application identifier for the tag selected by the reader session when discovering new tags.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var initialSelectedAID: String { get }
```

**Required**

## Discussion

The value matches one of the entries in the com.apple.developer.nfc.readersession.iso7816.select-identifiers information property list key.

## See Also

### Getting Tag Information

var identifier: Data

The unique hardware identifier of the tag.

**Required**

var historicalBytes: Data?

The historical bytes extracted from the Type A Answer To Select response.

**Required**

var applicationData: Data?

The application data bytes extracted from the Type B Answer To Request response.

**Required**

var proprietaryApplicationDataCoding: Bool

A Boolean value that indicates whether the application data follows proprietary data coding.

**Required**

