

- Media Library
- MLMediaSource
-  mediaObject(forIdentifier:) 

Instance Method

# mediaObject(forIdentifier:)

Returns the media object with the specified identifier.

Mac Catalyst 13.0+macOS 10.9–10.15Deprecated

``` source
func mediaObject(forIdentifier mediaObjectIdentifier: String) -> MLMediaObject?
```

## Parameters 

`mediaObjectIdentifier`  

The media object identifier to search for in the media source.

## Discussion

The media source must have finished loading before this method returns valid data. Specifically, the root media group must be available before the lookup methods will succeed. Otherwise, the return value is undefined.

## See Also

### Accessing Media

func mediaGroup(forIdentifier: String) -> MLMediaGroup?

Returns the media group with the specified identifier.

func mediaGroups(forIdentifiers: [String]) -> [String : MLMediaGroup]

Returns the media groups with the specified identifiers.

func mediaObjects(forIdentifiers: [String]) -> [String : MLMediaObject]

Returns the media objects with the specified identifiers.

