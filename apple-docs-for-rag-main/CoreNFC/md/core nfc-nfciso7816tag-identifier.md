

- Core NFC
- NFCISO7816Tag
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

var initialSelectedAID: String

A hexadecimal string of the application identifier for the tag selected by the reader session when discovering new tags.

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

