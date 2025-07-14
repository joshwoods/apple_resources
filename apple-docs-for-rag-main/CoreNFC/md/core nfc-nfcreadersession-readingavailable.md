

- Core NFC
- NFCReaderSession
-  readingAvailable 

Type Property

# readingAvailable

A Boolean value that determines whether the device supports NFC tag reading.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class var readingAvailable: Bool { get }
```

## Discussion

Before creating a reader session, always check the readingAvailable property to determine whether the user’s device supports scanning for and detecting NFC tags.

