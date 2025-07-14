

- WatchKit
- WKAudioFileAsset
-  artist Deprecated

Instance Property

# artist

The artist information for the audio file.

watchOS 2.0–6.0Deprecated

``` source
var artist: String? { get }
```

## Discussion

If you do not set the artist name directly at initialization time, the asset object obtains the information from the audio file’s metadata.

## See Also

### Getting the Asset’s Properties

var url: URL

The URL of the audio file.

Deprecated

var duration: TimeInterval

The duration (in seconds) of the audio file.

Deprecated

var title: String?

The title information for the audio file.

Deprecated

var albumTitle: String?

The album title information for the audio file.

Deprecated

