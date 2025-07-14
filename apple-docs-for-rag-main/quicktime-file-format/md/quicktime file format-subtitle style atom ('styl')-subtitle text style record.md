

- QuickTime File Format
- Subtitle style atom ('styl')
-  Subtitle text style record 

Data field

# Subtitle text style record

One or more records that provide details about the subtitle’s style.

## Overview

One record consists of the following fields.

Start character  
A 16-bit value that is the offset of the first character that is to use the style specified in this record. Zero (`0`) is the first character in the subtitle.

End character  
A 16-bit value that is the offset of the character that follows the last character to use this style.

Font identifier  
A 16-bit value that must be set to the same font identifier as in the font table (`'ftab'` extension).

Font face  
An 8-bit integer that indicates the font’s style. Set this field to `0` for normal text. You can enable other style options by using one or more of the bit masks listed in Text.

Font size  
An 8-bit value that specifies the font’s size. See Subtitle sample description for more information.

Foreground color  
A 32-bit RGBA color that specifies the text’s color. See Subtitle sample description for more information.

## See Also

### Data fields

Size

An unsigned 32-bit integer holding the size of the subtitle style atom.

Type

An unsigned 32-bit field.

Entry count

An unsigned 16-bit integer specifying how many subtitle text style records follow this entry count.

