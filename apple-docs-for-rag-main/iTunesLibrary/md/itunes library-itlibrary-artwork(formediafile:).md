

- iTunes Library
- ITLibrary
-  artwork(forMediaFile:) 

Instance Method

# artwork(forMediaFile:)

Retrieves the artwork from a media file that may or may not be in the iTunes library.

Mac Catalyst 14.0+macOS 10.13+

``` source
func artwork(forMediaFile mediaFileURL: URL) -> ITLibArtwork?
```

## Parameters 

`mediaFileURL`  

The URL of the media file whose artwork you want to retrieve. The media file may or may not be in the iTunes library.

## Return Value

An ITLibArtwork instance representing the media file artwork, or `nil` if the media file doesn’t contain any artwork or the system can’t extract the artwork.

