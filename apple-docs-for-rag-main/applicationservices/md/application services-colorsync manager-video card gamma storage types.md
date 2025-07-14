

- Application Services
- ColorSync Manager
-  Video Card Gamma Storage Types 

# Video Card Gamma Storage Types

Specify data storage type constants.

## Overview

A video card gamma profile tag can store gamma data either as a formula or as a table of values. You use a storage type constant to specify which data storage type the tag uses.

If the video card uses a different format than the format you specify (for example, the card uses data in table format and you supply data in formula format), ColorSync will adapt the data you supply to match the format the card expects.

### Version-Notes

Starting with version 2.5, ColorSync supports an optional profile tag for video card gamma. The tag specifies gamma information, stored either as a formula or in table format, to be loaded into the video card when the profile containing the tag is put into use. As of version 2.5, the only ColorSync function that attempts to take advantage of video card gamma data is CMSetProfileByAVID.

## Topics

### Constants

var cmVideoCardGammaTableType: Int

The video card gamma data is stored in a table format. See CMVideoCardGammaTable for a description of the table format.

var cmVideoCardGammaFormulaType: Int

The video card gamma tag data is stored as a formula. See CMVideoCardGammaFormula for a description of the formula format.

