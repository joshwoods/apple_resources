

- Core NFC
- NFCNDEFTag
-  queryNDEFStatus(completionHandler:) 

Instance Method

# queryNDEFStatus(completionHandler:)

Asks the reader session for the NDEF support status of the tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func queryNDEFStatus(completionHandler: @escaping (NFCNDEFStatus, Int, (any Error)?) -> Void)
```

``` source
func queryNDEFStatus() async throws -> (NFCNDEFStatus, Int)
```

**Required**

## Parameters 

`completionHandler`  

The handler invoked by the reader session that provides the NDEF support status. The handler has the following parameters:

status  
The NFCNDEFStatus of the tag.

capacity  
Indicates the maximum NDEF message size, in bytes, that you can store on the tag.

error  
An NSError object if the query fails; otherwise, `nil`.

The session calls `completionHandler` on the dispatch queue provided when creating the NFCNDEFReaderSession.

## See Also

### Getting the Tag Status

var isAvailable: Bool

A Boolean value that determines whether the NDEF tag is available in the current reader session.

**Required**

enum NFCNDEFStatus

Constants that indicate status for an NDEF tag.

