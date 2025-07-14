

- QuickTime File Format
- Subtitle sample data
-  Text 

Data field

# Text

The subtitle text.

## Overview

The subtitle text is Unicode text, encoded either as UTF-8 text or UTF-16 text beginning with a UTF-16 BYTE ORDER MARK (`'\uFEFF'`) in big or little endian order. There is no null termination for the text.

## See Also

### Data fields

Text size

A 16-bit word that specifies the length (number of bytes) of the subtitle text.

Sample extensions

One or more atoms containing additional information for selecting and drawing the subtitle.

