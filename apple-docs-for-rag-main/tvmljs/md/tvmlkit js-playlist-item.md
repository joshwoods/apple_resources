

- TVMLKit JS
- Playlist
-  item 

Instance Method

# item

Returns the media item located in the indicated array index.

tvOS 9.0+

``` source
MediaItem item(
    in int index
);
```

## Parameters 

`index`  

The array index for the `MediaItem`.

## Return Value

The MediaItem object located in the designated index location. This method returns `null` if the index is out of range.

## See Also

### Modifying the Playlist

length

The number of items in the playlist.

Playlist

Creates a new playlist object.

pop

Removes a media item from the end of a playlist.

push

Adds a media item to the end of a playlist.

splice

Deletes the indicated array elements and replaces them with the specified elements.

