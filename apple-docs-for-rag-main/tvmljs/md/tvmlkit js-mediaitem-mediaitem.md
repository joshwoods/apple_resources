

- TVMLKit JS
- MediaItem
-  MediaItem 

Instance Method

# MediaItem

Creates a new `MediaItem` object from the information stored in the URL location.

tvOS 9.0+

``` source
new MediaItem(
    in String type, 
    in optional String url
);
```

## Parameters 

`type`  

The type of media item to be created. Valid values are `audio` and `video`. The default is `video`.

`url`  

The URL pointing to the media item information.

## Return Value

Returns the `MediaItem` object found in the location specified by the URL.

