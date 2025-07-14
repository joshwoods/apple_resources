

- CarPlay
- CPNowPlayingTemplate
-  isAlbumArtistButtonEnabled 

Instance Property

# isAlbumArtistButtonEnabled

A Boolean value that indicates whether the album and artist string is a button.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var isAlbumArtistButtonEnabled: Bool { get set }
```

## Discussion

The Now Playing template displays a string above the playback control buttons that contains the album and artist names. Set this property to true to turn the string into a button that you can use to present more information about the current track. To respond to a user tapping the button, create an object that conforms to CPNowPlayingTemplateObserver and register it with the Now Playing template using the template’s add(_:) method.

The default value is false.

## See Also

### Managing Albums, Artists, and Up Next

var isUpNextButtonEnabled: Bool

A Boolean value that manages the display of the Up Next button.

var upNextTitle: String

The title for the Up Next button.

