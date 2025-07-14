

- CarPlay
- CPNowPlayingTemplateObserver
-  nowPlayingTemplateUpNextButtonTapped(\_:) 

Instance Method

# nowPlayingTemplateUpNextButtonTapped(\_:)

Tells the observer that the user tapped the Up Next button.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
optional func nowPlayingTemplateUpNextButtonTapped(_ nowPlayingTemplate: CPNowPlayingTemplate)
```

## Parameters 

`nowPlayingTemplate`  

The template that contains the button that the user tapped.

## Discussion

When CarPlay calls this method on your observer, you should push an instance of CPListTemplate—other template types are not supported when Now Playing is the visible template—on to your navigation stack that displays a list of upcoming or queued content.

## See Also

### Responding to User Interactions

func nowPlayingTemplateAlbumArtistButtonTapped(CPNowPlayingTemplate)

Tells the observer that the user tapped the Album-Artist button.

