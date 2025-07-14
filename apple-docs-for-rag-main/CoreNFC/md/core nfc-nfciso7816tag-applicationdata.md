

- Core NFC
- NFCISO7816Tag
-  applicationData 

Instance Property

# applicationData

The application data bytes extracted from the Type B Answer To Request response.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var applicationData: Data? { get }
```

**Required**

## See Also

### Getting Tag Information

var initialSelectedAID: String

A hexadecimal string of the application identifier for the tag selected by the reader session when discovering new tags.

**Required**

var identifier: Data

The unique hardware identifier of the tag.

**Required**

var historicalBytes: Data?

The historical bytes extracted from the Type A Answer To Select response.

**Required**

var proprietaryApplicationDataCoding: Bool

A Boolean value that indicates whether the application data follows proprietary data coding.

**Required**

