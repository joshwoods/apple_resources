

- Media Library
- MLMediaSource
-  mediaGroups(forIdentifiers:) 

Instance Method

# mediaGroups(forIdentifiers:)

Returns the media groups with the specified identifiers.

Mac Catalyst 13.0+macOS 10.9–10.15Deprecated

``` source
func mediaGroups(forIdentifiers mediaGroupIdentifiers: [String]) -> [String : MLMediaGroup]
```

## Parameters 

`mediaGroupIdentifiers`  

An array of media group identifiers to search for in the source.

## Return Value

A dictionary of media groups matching the specified identifiers.

## Discussion

The media source must have finished loading before this method returns valid data. Specifically, the root media group must be available before the lookup methods will succeed. Otherwise, the return value is undefined.

## See Also

### Accessing Media

func mediaGroup(forIdentifier: String) -> MLMediaGroup?

Returns the media group with the specified identifier.

func mediaObject(forIdentifier: String) -> MLMediaObject?

Returns the media object with the specified identifier.

func mediaObjects(forIdentifiers: [String]) -> [String : MLMediaObject]

Returns the media objects with the specified identifiers.

