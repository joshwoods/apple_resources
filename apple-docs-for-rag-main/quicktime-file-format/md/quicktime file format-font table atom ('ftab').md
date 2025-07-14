

- QuickTime File Format
-  Font table atom ('ftab') 

Atom

# Font table atom ('ftab')

An atom that specifies the font used to display the subtitle.

## Topics

### Data fields

Size

An unsigned 32-bit integer holding the size of the font table atom.

Type

An unsigned 32-bit field.

Count

An unsigned 16-bit integer specifying how many fonts are described in this table.

Font identifier

An unsigned 16-bit integer that identifies the font.

Font name length

An unsigned 8-bit integer specifying the length of the font name in bytes.

Font name

Must be either “Serif” or “Sans-Serif”.

## See Also

### Storing subtitles

Subtitle sample description

An atom that defines how to interpret subtitle media data.

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

