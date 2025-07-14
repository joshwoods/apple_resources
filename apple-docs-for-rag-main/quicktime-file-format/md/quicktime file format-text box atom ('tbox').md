

- QuickTime File Format
-  Text box atom ('tbox') 

Atom

# Text box atom ('tbox')

An atom that defines a text box for a subtitle sample.

## Overview

This optional extension defines a text box for a subtitle sample, to be used as described in Sample extensions. If present, this overrides the default text box in the associated sample description. If the subtitle sample description’s Display flags do not include the Vertical Placement flag (`0x20000000`), the Text Box atom should not be included in any sample of the subtitle track.

## Topics

### Data fields

Size

An unsigned 32-bit integer holding the size of the subtitle style atom.

Type

An unsigned 32-bit field.

Text box

A 64-bit rectangle that specifies an area to receive text (each 16 bits indicate top, left, bottom, and right, respectively) within the subtitle track.

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

Subtitle track header size and placement

Specify the size and placement of subtitles.

Referencing a related forced subtitle track

Prevent overlapping a timed subtitle track with a forced subtitle track.

