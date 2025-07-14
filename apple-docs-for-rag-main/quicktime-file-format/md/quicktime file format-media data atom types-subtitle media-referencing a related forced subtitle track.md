

- QuickTime File Format
- Media data atom types
- Subtitle media
-  Referencing a related forced subtitle track 

Article

# Referencing a related forced subtitle track

Prevent overlapping a timed subtitle track with a forced subtitle track.

## Overview

A subtitle track can contain a track reference of type `'forc'` to a paired subtitle track that contains only forced subtitles.

Pairing two subtitle tracks might be necessary if the timing of forced subtitle samples (see `'frcd'`) differs from the regular subtitle text, such as when a forced subtitle display would overlap in time with the display of the regular subtitle. If timings are the same, a single subtitle track should be used.

To pair two tracks, one subtitle track can contain any combination of forced and non-forced (regular) subtitle samples and the other track must contain only forced subtitles. The tracks must be in the same alternate group and be tagged with the same extended language tag and language code. The first, regular track then uses a track reference of type `'forc'` to reference the second, forced-only track. (Mixing extended language tags or codes for the same language in the same alternate group is undefined.)

Note

The regular track in a pair provides a complete transcription of the audio as subtitle text. This allows a user to listen in one language but to read subtitled dialogue in another language.

See Preparing sound and subtitle alternate groups for use with Apple devices and Track reference atom ('tref') for more information.

## See Also

### Storing subtitles

Subtitle sample description

An atom that defines how to interpret subtitle media data.

Font table atom ('ftab')

An atom that specifies the font used to display the subtitle.

Subtitle sample data

An atom that contains subtitle sample data.

Subtitle style atom ('styl')

An atom that specifies changes to the appearance of a subtitle.

Text box atom ('tbox')

An atom that defines a text box for a subtitle sample.

Subtitle track header size and placement

Specify the size and placement of subtitles.

