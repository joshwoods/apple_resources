

- QuickTime File Format
-  Text sample description 

Atom

# Text sample description

An atom that defines how to interpret text media data.

## Overview

The text sample description contains information that defines how to interpret text media data. This sample description is based on the standard sample description header, as described in Sample description atom ('stsd').

The data format field in the sample description is always set to `'text'`.

The text media handler also adds some of its own fields to the sample description.

## Topics

### Data fields

Display flags

A 32-bit integer containing flags that describe how the text should be drawn.

Text justification

A 32-bit integer that indicates how the text should be aligned.

Background color

A 48-bit RGB color that specifies the text’s background color.

Default text box

A 64-bit rectangle that specifies an area to receive text (top, left, bottom, right).

Reserved

A 64-bit value.

Font number

A 16-bit value.

Font face

A 16-bit integer that indicates the font’s style.

Reserved

An 8-bit value.

Reserved

A 16-bit value.

Foreground color

A 48-bit RGB color that specifies the text’s foreground color.

Text name

A Pascal string specifying the name of the font to use to display the text.

## See Also

### Storing text data

Text media information atom ('text')

An atom that contains information about text media.

Text sample data

An atom that contains text data.

Hypertext and wired text

Store hypertext in a text track sample atom.

