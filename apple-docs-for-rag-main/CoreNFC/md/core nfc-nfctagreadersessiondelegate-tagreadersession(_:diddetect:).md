

- Core NFC
- NFCTagReaderSessionDelegate
-  tagReaderSession(\_:didDetect:) 

Instance Method

# tagReaderSession(\_:didDetect:)

Tells the delegate that the session detected NFC tags.

iOS 13.0+iPadOS 13.0+Mac Catalyst

``` source
func tagReaderSession(
    _ session: NFCTagReaderSession,
    didDetect tags: [NFCTag]
)
```

**Required**

## Parameters 

`session`  

The session that detected the tags.

`tags`  

An array of NFC tags detected by the session.

## Discussion

The polling options specified when creating an NFCTagReaderSession object determine the types of tags that the session can detect.

