

- CarPlay
-  CPNowPlayingMoreButton 

Class

# CPNowPlayingMoreButton

A button for presenting more options to the user.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPNowPlayingMoreButton
```

## Overview

`CPNowPlayingMoreButton` is a concrete subclass of CPNowPlayingButton. Use this button to present a CPListTemplate, CPAlertTemplate, or another contextual interface for the currently playing item. For example, if the item is a podcast, use the button’s handler to present a template that displays the episode’s show notes.

## Relationships

### Inherits From

- CPNowPlayingButton

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Managing the Template’s Buttons

var nowPlayingButtons: [CPNowPlayingButton]

The Now Playing template’s playback control buttons.

func updateNowPlayingButtons([CPNowPlayingButton])

Updates the playback control buttons the template displays.

class CPNowPlayingButton

The abstract base class that Now Playing template buttons use.

class CPNowPlayingImageButton

A button that displays an image.

class CPNowPlayingAddToLibraryButton

A button for adding the current playing item to a collection.

class CPNowPlayingPlaybackRateButton

A button for cycling through the available playback rates.

class CPNowPlayingRepeatButton

A button for cycling through the available repeat modes.

class CPNowPlayingShuffleButton

A button for cycling through the available shuffle modes.

