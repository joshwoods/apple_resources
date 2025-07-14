

- Core NFC
- NFCNDEFTag
-  readNDEF(completionHandler:) 

Instance Method

# readNDEF(completionHandler:)

Retrieves an NDEF message from the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func readNDEF(completionHandler: @escaping (NFCNDEFMessage?, (any Error)?) -> Void)
```

``` source
func readNDEF() async throws -> NFCNDEFMessage
```

**Required**

## Parameters 

`completionHandler`  

The handler invoked by the reader session that provides the NDEF message. The handler has the following parameters:

message  
An NFCNDEFMessage object, or `nil` if an error occurs while retrieving the message.

error  
An NSError object if the read request fails; otherwise, `nil`.

The session calls `completionHandler` on the dispatch queue provided when creating the NFCNDEFReaderSession.

