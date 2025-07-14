

- QuickTime File Format
-  Subtitle sample data 

Atom

# Subtitle sample data

An atom that contains subtitle sample data.

## Mentioned in 

Preparing sound and subtitle alternate groups for use with Apple devices

## Overview

Subtitle sample data consists of a 16-bit word that specifies the length (number of bytes) of the subtitle text, followed by the subtitle text and then by optional sample extensions. The subtitle text is Unicode text, encoded either as UTF-8 text or UTF-16 text beginning with a UTF-16 BYTE ORDER MARK (`'\uFEFF'`) in big or little endian order. There is no null termination for the text.

Following the subtitle text, there may be one or more atoms containing additional information for selecting and drawing the subtitle.

## Topics

### Data fields

Text size

A 16-bit word that specifies the length (number of bytes) of the subtitle text.

Text

The subtitle text.

Sample extensions

One or more atoms containing additional information for selecting and drawing the subtitle.

## See Also

### Storing subtitles

Subtitle sample description

An atom that defines how to interpret subtitle media data.

Font table atom ('ftab')

An atom that specifies the font used to display the subtitle.

Subtitle style atom ('styl')

An atom that specifies changes to the appearance of a subtitle.

Text box atom ('tbox')

An atom that defines a text box for a subtitle sample.

Subtitle track header size and placement

Specify the size and placement of subtitles.

Referencing a related forced subtitle track

Prevent overlapping a timed subtitle track with a forced subtitle track.

