

- Core NFC
- NFCNDEFReaderSession
-  connect(to:completionHandler:) 

Instance Method

# connect(to:completionHandler:)

Connects the reader session to a tag and activates that tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func connect(
    to tag: any NFCNDEFTag,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func connect(to tag: any NFCNDEFTag) async throws
```

## Parameters 

`tag`  

A tag that the reader session should attempt connecting to.

`completionHandler`  

A handler that the reader session invokes after completing the tag-connect request. The handler has the following parameter:

error  
`nil` when the session successfully connects to the tag; otherwise, an NSError object.

The session calls `completionHandler` on the dispatch queue provided when creating the NFCNDEFReaderSession.

## Discussion

A tag stays connected until your app connects to a different tag or restarts polling. Connecting to a tag that is already connected has no effect.

