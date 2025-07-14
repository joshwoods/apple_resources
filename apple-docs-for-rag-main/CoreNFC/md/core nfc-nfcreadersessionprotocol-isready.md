

- Core NFC
- NFCReaderSessionProtocol
-  isReady 

Instance Property

# isReady

A Boolean value that indicates whether the reader session is started and ready to use.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var isReady: Bool { get }
```

**Required**

## Discussion

As soon as a reader session is successfully activated, radio-frequency discovery polling begins. When a tag is detected, readerSession:didDetectTags: is called.

