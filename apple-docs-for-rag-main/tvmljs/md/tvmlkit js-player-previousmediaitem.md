

- TVMLKit JS
- Player
-  previousMediaItem 

Instance Property

# previousMediaItem

The item in the playlist previous to the currently selected item.

tvOS 9.0+

``` source
readonly attribute MediaItem previousMediaItem;
```

## Discussion

This property returns `null` if there are no items in the playlist previous to the currently playing item.

## See Also

### Inspecting Media Items

currentMediaItem

The currently selected media item in the playlist.

currentMediaItemDate

Contains the current time of the media item as a `Date` object.

currentMediaItemDuration

The length, in seconds, of the current media item.

nextMediaItem

The next media item in the playlist after the currently selected item.

