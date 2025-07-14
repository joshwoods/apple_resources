

- Core NFC
- NFCNDEFTag
-  writeLock(completionHandler:) 

Instance Method

# writeLock(completionHandler:)

Changes the NDEF tag status to read-only, preventing future write operations.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func writeLock(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func writeLock() async throws
```

**Required**

## Parameters 

`completionHandler`  

The handler invoked by the reader session after completing the lock request. The session calls `completionHandler` on the dispatch queue provided when creating the NFCNDEFReaderSession.

The handler has the following parameter:

error  
An NSError object if the write request fails. A value of `nil` indicates that the session locked the tag and future write requests aren’t possible.

## Discussion

Calling this method updates the write access condition byte in the NDEF File Control of the tag’s file system, thus locking the tag. This is a permanent action that you cannot undo. After locking the tag, you can no longer write data to it.

## See Also

### Writing to the Tag

func writeNDEF(NFCNDEFMessage, completionHandler: ((any Error)?) -> Void)

Saves an NDEF message to a writable tag.

**Required**

