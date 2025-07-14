

- ProximityReader
- MobileDocumentReader
- MobileDocumentReader.Configuration
-  readerInstanceIdentifier 

Instance Property

# readerInstanceIdentifier

The unique identifier for the mobile document reader instance.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
let readerInstanceIdentifier: String
```

## Mentioned in 

Generating reader tokens for the Verifier API

## Discussion

Note

Do not cache this value. When generating a reader token always retrieve the latest reader instance identifier first.

