

- CarPlay
- CPNowPlayingTemplateObserver
-  nowPlayingTemplateAlbumArtistButtonTapped(\_:) 

Instance Method

# nowPlayingTemplateAlbumArtistButtonTapped(\_:)

Tells the observer that the user tapped the Album-Artist button.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
optional func nowPlayingTemplateAlbumArtistButtonTapped(_ nowPlayingTemplate: CPNowPlayingTemplate)
```

## Parameters 

`nowPlayingTemplate`  

The template that contains the button that the user tapped.

## Discussion

When CarPlay calls this method on your observer, you should present or push a new template that displays the content of the current album, playlist or podcast.

## See Also

### Responding to User Interactions

func nowPlayingTemplateUpNextButtonTapped(CPNowPlayingTemplate)

Tells the observer that the user tapped the Up Next button.

