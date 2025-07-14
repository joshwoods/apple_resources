

- TVMLKit JS
- Playlist
-  splice 

Instance Method

# splice

Deletes the indicated array elements and replaces them with the specified elements.

tvOS 9.0+

``` source
Array splice(
    in int start, 
    in int deleteCount, 
    in Object elements
);
```

## Parameters 

`index`  

The array index indicating the beginning of the splice to be deleted.

`howMany`  

The length of the splice, in number of elements.

`elements`  

An array of new elements that are replacing the deleted elements.

## Return Value

An array of the deleted elements.

## Discussion

Use this method to modify the contents of the playlist.

## See Also

### Modifying the Playlist

item

Returns the media item located in the indicated array index.

length

The number of items in the playlist.

Playlist

Creates a new playlist object.

pop

Removes a media item from the end of a playlist.

push

Adds a media item to the end of a playlist.

