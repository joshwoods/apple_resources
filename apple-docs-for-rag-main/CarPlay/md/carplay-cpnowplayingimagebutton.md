

- CarPlay
-  CPNowPlayingImageButton 

Class

# CPNowPlayingImageButton

A button that displays an image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPNowPlayingImageButton
```

## Overview

`CPNowPlayingImageButton` is a concrete subclass of CPNowPlayingButton. Use this class when you want to display a button that contains an image.

In iOS 17 and later, CarPlay retints the custom now playing image buttons your app provides; you need to provide images as monocolor assets.

CarPlay doesn’t support animated images. If you provide an animated image, CarPlay uses only the first image in the animation sequence.

To properly size your image, use the display scale of the vehicle’s primary screen—see your interface controller’s carTraitCollection property—and make sure it is no larger than CPNowPlayingButtonMaximumImageSize.

## Topics

### Creating a Button

init(image: UIImage, handler: ((CPNowPlayingButton) -> Void)?)

Creates a Now Playing button that displays a custom image and invokes a handler.

let CPNowPlayingButtonMaximumImageSize: CGSize

The maximum size CarPlay supports for a button’s image.

### Getting the Button’s Image

var image: UIImage?

The image that the button displays.

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

