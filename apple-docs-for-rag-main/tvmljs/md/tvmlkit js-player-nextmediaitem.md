

- TVMLKit JS
- Player
-  nextMediaItem 

Instance Property

# nextMediaItem

The next media item in the playlist after the currently selected item.

tvOS 9.0+

``` source
readonly attribute MediaItem nextMediaItem;
```

## Discussion

This property returns `null` if the current item is the last item in the playlist.

## See Also

### Inspecting Media Items

currentMediaItem

The currently selected media item in the playlist.

currentMediaItemDate

Contains the current time of the media item as a `Date` object.

currentMediaItemDuration

The length, in seconds, of the current media item.

previousMediaItem

The item in the playlist previous to the currently selected item.

