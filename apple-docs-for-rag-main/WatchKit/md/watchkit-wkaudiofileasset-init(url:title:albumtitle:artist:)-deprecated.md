

- WatchKit
- WKAudioFileAsset
-  init(url:title:albumTitle:artist:) Deprecated

Initializer

# init(url:title:albumTitle:artist:)

Returns an audio file asset and sets the metadata for that item.

watchOS 2.0–6.0Deprecated

``` source
convenience init(
    url URL: URL,
    title: String?,
    albumTitle: String?,
    artist: String?
)
```

## Parameters 

`URL`  

A file-based URL that identifies the audio file. This URL must refer to a shared location that can be accessed by both the Watch app interface and the WatchKit extension. For more information, see Sharing Data in App Programming Guide for watchOS.

This parameter must not be `nil`.

`title`  

The title to use for the audio file asset. Specify `nil` to use the title information from the file’s metadata. If you specify `nil` and no title is found in the metadata, the title is set to the file’s name.

`albumTitle`  

The album title to use for the audio file asset. Specify `nil` to use the album title information from the file’s metadata.

`artist`  

The artist to use for the audio file asset. Specify `nil` to use the artist information from the file’s metadata.

## Return Value

An initialized asset object.

## See Also

### Creating an Asset

convenience init(url: URL)

Returns an asset for the audio file at the specified URL.

Deprecated

