

- Core NFC
- NFCTagReaderSession
-  connect(to:completionHandler:) 

Instance Method

# connect(to:completionHandler:)

Connects the reader session to a tag and activates that tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst

``` source
func connect(
    to tag: NFCTag,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

## Parameters 

`tag`  

A tag to which the reader session should attempt to connect.

`completionHandler`  

A handler that the reader session invokes after completing the tag-connect request. The handler has the following parameter:

error  
`nil` when the session successfully connects to the tag; otherwise, an Error object.

The session calls `completionHandler` on the dispatch queue provided when creating the NFCTagReaderSession.

## Discussion

A tag stays connected until your app connects to a different tag or restarts polling. Connecting to a tag that is already connected has no effect.

## See Also

### Connecting to a Tag

var connectedTag: NFCTag?

The tag connected to the reader session.

