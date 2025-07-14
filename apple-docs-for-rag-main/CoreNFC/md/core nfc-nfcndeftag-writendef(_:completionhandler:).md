

- Core NFC
- NFCNDEFTag
-  writeNDEF(\_:completionHandler:) 

Instance Method

# writeNDEF(\_:completionHandler:)

Saves an NDEF message to a writable tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func writeNDEF(
    _ ndefMessage: NFCNDEFMessage,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func writeNDEF(_ ndefMessage: NFCNDEFMessage) async throws
```

**Required**

## Parameters 

`ndefMessage`  

The NDEF message to write to the tag.

`completionHandler`  

The handler invoked by the reader session after completing the write request. The session calls `completionHandler` on the dispatch queue provided when creating the NFCNDEFReaderSession.

The handler has the following parameter:

error  
An NSError object if the write request fails. A value of `nil` indicates that the write was successful.

## Discussion

To determine whether the tag is writable, call queryNDEFStatus(completionHandler:) and check that the `status` is NFCNDEFStatus.readWrite.

## See Also

### Writing to the Tag

func writeLock(completionHandler: ((any Error)?) -> Void)

Changes the NDEF tag status to read-only, preventing future write operations.

**Required**

