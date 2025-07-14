

- CarPlay
-  CPNowPlayingAddToLibraryButton 

Class

# CPNowPlayingAddToLibraryButton

A button for adding the current playing item to a collection.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPNowPlayingAddToLibraryButton
```

## Overview

`CPNowPlayingAddToLibraryButton` is a concrete subclass of CPNowPlayingButton. Use this button to allow a user to add the current playing item to a collection, such as their library. You implement this functionality in the button’s handler, or use the handler to invoke existing code that performs this function.

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

class CPNowPlayingMoreButton

A button for presenting more options to the user.

class CPNowPlayingPlaybackRateButton

A button for cycling through the available playback rates.

class CPNowPlayingRepeatButton

A button for cycling through the available repeat modes.

class CPNowPlayingShuffleButton

A button for cycling through the available shuffle modes.

