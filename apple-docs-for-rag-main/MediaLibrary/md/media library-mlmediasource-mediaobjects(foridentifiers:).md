

- Media Library
- MLMediaSource
-  mediaObjects(forIdentifiers:) 

Instance Method

# mediaObjects(forIdentifiers:)

Returns the media objects with the specified identifiers.

Mac Catalyst 13.0+macOS 10.9–10.15Deprecated

``` source
func mediaObjects(forIdentifiers mediaObjectIdentifiers: [String]) -> [String : MLMediaObject]
```

## Parameters 

`mediaObjectIdentifiers`  

An array of media object identifiers to search for in the source.

## Return Value

A dictionary of media objects matching the specified identifiers.

## Discussion

The media source must have finished loading before this method returns valid data. Specifically, the root media group must be available before the lookup methods will succeed. Otherwise, the return value is undefined.

## See Also

### Accessing Media

func mediaGroup(forIdentifier: String) -> MLMediaGroup?

Returns the media group with the specified identifier.

func mediaGroups(forIdentifiers: [String]) -> [String : MLMediaGroup]

Returns the media groups with the specified identifiers.

func mediaObject(forIdentifier: String) -> MLMediaObject?

Returns the media object with the specified identifier.

