

- Core Media
-  kCMTextDisplayFlag_allSubtitlesForced 

Global Variable

# kCMTextDisplayFlag_allSubtitlesForced

A flag that describes treating all subtitle samples as if they contain forced subtitles.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var kCMTextDisplayFlag_allSubtitlesForced: CMTextDisplayFlags { get }
```

## See Also

### Constants

var kCMTextDisplayFlag_scrollIn: CMTextDisplayFlags

A flag that describes the text scrolls into the display region.

var kCMTextDisplayFlag_scrollOut: CMTextDisplayFlags

A flag that describes the text scrolls out of the display region.

var kCMTextDisplayFlag_scrollDirectionMask: CMTextDisplayFlags

A flag that describes the scrolling direction is set by a two-bit field, obtained from displayFlags using kCMTextDisplayFlag_scrollDirectionMask.

var kCMTextDisplayFlag_scrollDirection_bottomToTop: CMTextDisplayFlags

A flag that describes the text is vertically scrolled up (“credits style”), entering from the bottom and leaving towards the top.

var kCMTextDisplayFlag_scrollDirection_rightToLeft: CMTextDisplayFlags

A flag that describes the text is horizontally scrolled (“marquee style”), entering from the right and leaving towards the left.

var kCMTextDisplayFlag_scrollDirection_topToBottom: CMTextDisplayFlags

A flag that describes the text is vertically scrolled down, entering from the top and leaving towards the bottom.

var kCMTextDisplayFlag_scrollDirection_leftToRight: CMTextDisplayFlags

A flag that describes the text is horizontally scrolled, entering from the left and leaving towards the right.

var kCMTextDisplayFlag_continuousKaraoke: CMTextDisplayFlags

A flag that describes enabling the continuous karaoke mode where the range of karaoke highlighting extends to include additional ranges rather than the highlighting moves onto the next range.

var kCMTextDisplayFlag_writeTextVertically: CMTextDisplayFlags

A flag that describes the text renders vertically.

var kCMTextDisplayFlag_fillTextRegion: CMTextDisplayFlags

A flag that describes the subtitle display bounds are to be filled with the color specified by `kCMTextFormatDescriptionExtension_BackgroundColor`.

var kCMTextDisplayFlag_forcedSubtitlesPresent: CMTextDisplayFlags

A flag that describes forcing subtitles are present, for example, a subtitle which only displays during foreign language sections of the video. Check individual samples to determine what type of subtitle is contained.

