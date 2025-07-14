

- QuickTime File Format
-  Subtitle sample description 

Atom

# Subtitle sample description

An atom that defines how to interpret subtitle media data.

## Overview

The subtitle sample description contains information that defines how to interpret subtitle media data. This sample description is based on the standard sample description header, as described in Sample description atom ('stsd').

Note

Only one sample description is permitted in a `'sbtl'` track.

The data format field in the sample description is currently always set to `'tx3g'`. Unrecognized data formats should be ignored. The text media described here is based on the text box defined in the 3GPP Timed Text specification but provides a different track type and media handler designed specifically for subtitles.

The subtitle media handler adds some of its own fields to the sample description.

## Topics

### Data fields

Display flags

A 32-bit integer containing flags that describe how the subtitle text should be drawn.

Reserved

An 8-bit integer.

Reserved

An 8-bit integer.

Reserved

A 32-bit integer.

Default text box

A 64-bit rectangle that specifies an area to receive text (each 16 bits indicate top, left, bottom, and right, respectively) within the subtitle track.

Reserved

A 32-bit value.

Font identifier

A 16-bit value that must be set to the same font identifier as in the font table.

Font face

An 8-bit integer that indicates the font’s style.

Font size

An 8-bit value for the font size, expressed in points.

Foreground color

A 32-bit RGBA color that specifies the text’s color, 8 bits each for red, green, blue, and alpha (transparency).

Font table

An atom that identifies the font to use to display the text.

## See Also

### Storing subtitles

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

Referencing a related forced subtitle track

Prevent overlapping a timed subtitle track with a forced subtitle track.

