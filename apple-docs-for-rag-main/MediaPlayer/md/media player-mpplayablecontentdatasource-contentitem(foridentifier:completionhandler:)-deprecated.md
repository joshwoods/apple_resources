

- Media Player
- MPPlayableContentDataSource
-  contentItem(forIdentifier:completionHandler:) Deprecated

Instance Method

# contentItem(forIdentifier:completionHandler:)

Retrieves the content item associated with the provided identifier.

iOS 10.0–14.0DeprecatediPadOS 10.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func contentItem(
    forIdentifier identifier: String,
    completionHandler: @escaping (MPContentItem?, (any Error)?) -> Void
)
```

``` source
optional func contentItem(forIdentifier identifier: String) async throws -> MPContentItem
```

Deprecated

Use CarPlay framework

## Parameters 

`identifier`  

The String that identifies a content item.

`completionHandler`  

A block that is called after the content item has been loaded.

contentItem  
The content item associated with the identifier. If there is no content item, the value of this parameter is `nil`.

error  
If an error occurred, this parameter holds the error object that explains the error. Otherwise, the value of this parameter is `nil`.

## Discussion

Client apps should always call the completion handler after loading has finished.

## See Also

### Retrieving a media item

func contentItem(at: IndexPath) -> MPContentItem?

Retrieves the media item at the specified index.

**Required**

Deprecated

