

- QuickTime File Format
- Movie profile atom ('prfl')
-  Feature code 

Data field

# Feature code

A 32-bit unsigned integer that represents a code specifying a feature.

## Overview

The third field is the feature code, or name, a 32-bit unsigned integer that is usually best interpreted as four ASCII characters. Example: the maximum video bit rate feature has a feature code or name of `'mvbr'`. It is permissible to use a feature code value of zero (`0x00000000`, not four ASCII zero characters) as a placeholder in one or more name-value pairs. The reader should ignore feature codes of value zero.

## See Also

### Data fields

Reserved

A 32-bit field.

Part-ID

A 32-bit field that defines the feature as being either brand-specific or universal.

Value

A 32-bit field that represents a value related to a feature.

