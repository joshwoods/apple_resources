

- WebKit JS
- HTMLMediaElement
-  Media Ready States 

API Collection

# Media Ready States

Possible values for the readyState property.

## Topics

### Constants

HAVE_NOTHING

No media data is available for playback at the current time.

HAVE_METADATA

Enough of the media resource has been loaded to know the duration, and in the case of a `video` element, the dimensions.

HAVE_CURRENT_DATA

Data for the current playback position is available, but not enough to begin playback.

HAVE_FUTURE_DATA

Enough data is available to begin playback.

HAVE_ENOUGH_DATA

Enough data is available to play at the default playback rate to the end of the media resource without having to pause to rebuffer.

