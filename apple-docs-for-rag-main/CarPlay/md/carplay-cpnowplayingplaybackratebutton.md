

- CarPlay
-  CPNowPlayingPlaybackRateButton 

Class

# CPNowPlayingPlaybackRateButton

A button for cycling through the available playback rates.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPNowPlayingPlaybackRateButton
```

## Overview

`CPNowPlayingPlaybackRateButton` is a concrete subclass of CPNowPlayingButton. Use the button’s handler to invoke your existing functionality for cycling through playback rates, using the same MPChangePlaybackRateCommand that you provide to MPRemoteCommandCenter.

CarPlay uses `MPRemoteCommandCenter` to observe changes to the playback rate and updates the button’s appearance accordingly.

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

class CPNowPlayingMoreButton

A button for presenting more options to the user.

class CPNowPlayingRepeatButton

A button for cycling through the available repeat modes.

class CPNowPlayingShuffleButton

A button for cycling through the available shuffle modes.

