

- Media Player
- MPMediaPlaylistCreationMetadata
-  authorDisplayName 

Instance Property

# authorDisplayName

App defined display name for the playlist.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+visionOS 1.0+

``` source
var authorDisplayName: String! { get set }
```

## Discussion

The system requires this property for 3rd party apps. Defaults to the app display name when not defined.

## See Also

### Metadata for a playlist

var descriptionText: String

The descriptive text for the playlist.

var name: String

The playlist’s displayed name.

