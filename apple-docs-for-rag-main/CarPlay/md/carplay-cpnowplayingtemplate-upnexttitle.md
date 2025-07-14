

- CarPlay
- CPNowPlayingTemplate
-  upNextTitle 

Instance Property

# upNextTitle

The title for the Up Next button.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var upNextTitle: String { get set }
```

## Discussion

If you display the Up Next button in your app by setting isUpNextButtonEnabled to true, use this property to set the button’s title. If you don’t specify a title, CarPlay uses the system default title.

## See Also

### Managing Albums, Artists, and Up Next

var isAlbumArtistButtonEnabled: Bool

A Boolean value that indicates whether the album and artist string is a button.

var isUpNextButtonEnabled: Bool

A Boolean value that manages the display of the Up Next button.

