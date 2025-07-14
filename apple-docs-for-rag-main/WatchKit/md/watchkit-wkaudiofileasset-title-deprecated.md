

- WatchKit
- WKAudioFileAsset
-  title Deprecated

Instance Property

# title

The title information for the audio file.

watchOS 2.0–6.0Deprecated

``` source
var title: String? { get }
```

## Discussion

If you do not set the title directly at initialization time, the asset object obtains the information from the audio file’s metadata. If the file does not contain any title metadata, the filename is used for the title.

## See Also

### Getting the Asset’s Properties

var url: URL

The URL of the audio file.

Deprecated

var duration: TimeInterval

The duration (in seconds) of the audio file.

Deprecated

var albumTitle: String?

The album title information for the audio file.

Deprecated

var artist: String?

The artist information for the audio file.

Deprecated

