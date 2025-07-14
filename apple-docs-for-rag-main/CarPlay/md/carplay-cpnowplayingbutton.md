

- CarPlay
-  CPNowPlayingButton 

Class

# CPNowPlayingButton

The abstract base class that Now Playing template buttons use.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPNowPlayingButton
```

## Overview

`CPNowPlayingButton` is an abstract base class for defining buttons that the Now Playing template displays. It provides the common functionality that’s present in all buttons available to the template.

You don’t use this class directly, or create your own subclasses. Instead, you must use one of the concrete subclasses that the framework provides, such as CPNowPlayingImageButton or CPNowPlayingShuffleButton.

## Topics

### Creating a Button

init(handler: ((CPNowPlayingButton) -> Void)?)

Creates a Now Playing button that invokes a handler.

### Managing the Button State

var isEnabled: Bool

A Boolean value that indicates whether the button is in an enabled state.

var isSelected: Bool

A Boolean value that indicates whether the button is in a selected state.

## Relationships

### Inherits From

- NSObject

### Inherited By

- CPNowPlayingAddToLibraryButton
- CPNowPlayingImageButton
- CPNowPlayingMoreButton
- CPNowPlayingPlaybackRateButton
- CPNowPlayingRepeatButton
- CPNowPlayingShuffleButton

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

