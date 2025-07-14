

- QuickTime File Format
-  Subtitle style atom ('styl') 

Atom

# Subtitle style atom ('styl')

An atom that specifies changes to the appearance of a subtitle.

## Overview

This extension specifies changes to the appearance of a subtitle. The style information in the subtitle sample description provides the default style for the subtitle text. This extension allows you to override the default style for different parts, or all, of the subtitle text.

## Topics

### Data fields

Size

An unsigned 32-bit integer holding the size of the subtitle style atom.

Type

An unsigned 32-bit field.

Entry count

An unsigned 16-bit integer specifying how many subtitle text style records follow this entry count.

Subtitle text style record

One or more records that provide details about the subtitle’s style.

## See Also

### Storing subtitles

Subtitle sample description

An atom that defines how to interpret subtitle media data.

Font table atom ('ftab')

An atom that specifies the font used to display the subtitle.

Subtitle sample data

An atom that contains subtitle sample data.

Text box atom ('tbox')

An atom that defines a text box for a subtitle sample.

Subtitle track header size and placement

Specify the size and placement of subtitles.

Referencing a related forced subtitle track

Prevent overlapping a timed subtitle track with a forced subtitle track.

