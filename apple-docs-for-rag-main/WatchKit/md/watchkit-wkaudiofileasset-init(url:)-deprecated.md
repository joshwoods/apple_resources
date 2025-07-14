

- WatchKit
- WKAudioFileAsset
-  init(url:) Deprecated

Initializer

# init(url:)

Returns an asset for the audio file at the specified URL.

watchOS 2.0–6.0Deprecated

``` source
convenience init(url URL: URL)
```

## Parameters 

`URL`  

A file-based URL that identifies the audio file. This URL must refer to a shared location that can be accessed by both the Watch app interface and the WatchKit extension. For more information, see Sharing Data in App Programming Guide for watchOS.

This parameter must not be `nil`.

## Return Value

An initialized asset object.

## Discussion

This method creates an asset for the specified media file. The audio file’s title, album title, and artist information are derived from the metadata in the audio file itself.

## See Also

### Creating an Asset

convenience init(url: URL, title: String?, albumTitle: String?, artist: String?)

Returns an audio file asset and sets the metadata for that item.

Deprecated

