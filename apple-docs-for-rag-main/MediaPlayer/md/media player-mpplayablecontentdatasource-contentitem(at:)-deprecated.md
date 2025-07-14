

- Media Player
- MPPlayableContentDataSource
-  contentItem(at:) Deprecated

Instance Method

# contentItem(at:)

Retrieves the media item at the specified index.

iOS 7.1–14.0DeprecatediPadOS 7.1–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func contentItem(at indexPath: IndexPath) -> MPContentItem?
```

**Required**

Deprecated

Use CarPlay framework

## Parameters 

`indexPath`  

The index for the media item to be retrieved.

## Return Value

The media item at the indicated index.

## See Also

### Retrieving a media item

func contentItem(forIdentifier: String, completionHandler: (MPContentItem?, (any Error)?) -> Void)

Retrieves the content item associated with the provided identifier.

Deprecated

