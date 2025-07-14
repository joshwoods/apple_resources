

- CarPlay
- CPNowPlayingTemplate
-  updateNowPlayingButtons(\_:) 

Instance Method

# updateNowPlayingButtons(\_:)

Updates the playback control buttons the template displays.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func updateNowPlayingButtons(_ nowPlayingButtons: [CPNowPlayingButton])
```

## Parameters 

`nowPlayingButtons`  

The array of buttons to display.

## Discussion

You can provide a maximum of five playback control buttons. The template arranges the buttons using the array’s order, from the leading edge of the CarPlay screen to the trailing edge.

## See Also

### Managing the Template’s Buttons

var nowPlayingButtons: [CPNowPlayingButton]

The Now Playing template’s playback control buttons.

class CPNowPlayingButton

The abstract base class that Now Playing template buttons use.

class CPNowPlayingImageButton

A button that displays an image.

class CPNowPlayingAddToLibraryButton

A button for adding the current playing item to a collection.

class CPNowPlayingMoreButton

A button for presenting more options to the user.

class CPNowPlayingPlaybackRateButton

A button for cycling through the available playback rates.

class CPNowPlayingRepeatButton

A button for cycling through the available repeat modes.

class CPNowPlayingShuffleButton

A button for cycling through the available shuffle modes.

