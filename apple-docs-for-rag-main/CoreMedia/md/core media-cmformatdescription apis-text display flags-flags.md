

- Core Media
- CMFormatDescription APIs
-  Text Display Flags 

API Collection

# Text Display Flags

Flags that identify text display methods.

## Topics

### Constants

var kCMTextDisplayFlag_allSubtitlesForced: CMTextDisplayFlags

A flag that describes treating all subtitle samples as if they contain forced subtitles.

var kCMTextDisplayFlag_continuousKaraoke: CMTextDisplayFlags

A flag that describes enabling the continuous karaoke mode where the range of karaoke highlighting extends to include additional ranges rather than the highlighting moves onto the next range.

var kCMTextDisplayFlag_fillTextRegion: CMTextDisplayFlags

A flag that describes the subtitle display bounds are to be filled with the color specified by `kCMTextFormatDescriptionExtension_BackgroundColor`.

var kCMTextDisplayFlag_forcedSubtitlesPresent: CMTextDisplayFlags

A flag that describes forcing subtitles are present, for example, a subtitle which only displays during foreign language sections of the video. Check individual samples to determine what type of subtitle is contained.

var kCMTextDisplayFlag_obeySubtitleFormatting: CMTextDisplayFlags

A flag that describes using the subtitle display bounds to determine if the system places the subtitltes near the top or bottom of the video.

var kCMTextDisplayFlag_scrollDirectionMask: CMTextDisplayFlags

A flag that describes the scrolling direction is set by a two-bit field, obtained from displayFlags using kCMTextDisplayFlag_scrollDirectionMask.

var kCMTextDisplayFlag_scrollDirection_bottomToTop: CMTextDisplayFlags

A flag that describes the text is vertically scrolled up (“credits style”), entering from the bottom and leaving towards the top.

var kCMTextDisplayFlag_scrollDirection_leftToRight: CMTextDisplayFlags

A flag that describes the text is horizontally scrolled, entering from the left and leaving towards the right.

var kCMTextDisplayFlag_scrollDirection_rightToLeft: CMTextDisplayFlags

A flag that describes the text is horizontally scrolled (“marquee style”), entering from the right and leaving towards the left.

var kCMTextDisplayFlag_scrollDirection_topToBottom: CMTextDisplayFlags

A flag that describes the text is vertically scrolled down, entering from the top and leaving towards the bottom.

var kCMTextDisplayFlag_scrollIn: CMTextDisplayFlags

A flag that describes the text scrolls into the display region.

var kCMTextDisplayFlag_scrollOut: CMTextDisplayFlags

A flag that describes the text scrolls out of the display region.

var kCMTextDisplayFlag_writeTextVertically: CMTextDisplayFlags

A flag that describes the text renders vertically.

## See Also

### Constants

Format Description Error Codes

Errors the system returns from format description calls.

Format Description Bridge Error Codes

Bridge errors the system returns from format description calls.

Format Description Constants

Constants that identify format descriptions.

Text Format Description Constants

Constants that identify text format descriptions.

Metadata Format Description Constants

Constants that identify metadata format descriptions.

Time Code Format Description Constants

Constants that identify time code format descriptions.

Pixel Aspect Ratio Extension Constants

Constants that identify pixel aspect ratio extensions.

Chroma Location Extension Constants

Constants that identify chroma location extensions.

Clean Aperture Extension Constants

Constants that identify clean aperture extensions.

Color Primary Extension Constants

Constants that identify color primary extensions.

Field Detail Extension Constants

Constants that identify field detail extensions.

Transfer Function Extension Constants

Constants that identify transfer function extensions.

MPEG-2-conformant Formats

Constants that identify MPEG-2 formats.

HEVC Temporal Level Info Constants

Constants that identify HEVC temporal level information.

YCbCrMatrix Extension Constants

Constants that identify YCbCrMatrix extensions.

