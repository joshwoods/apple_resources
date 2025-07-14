

- Core Services
- Carbon Core
- Unicode Utilities
-  Text Boundary Operation Class 

# Text Boundary Operation Class

Identifies the class of Unicode utility operations that find text boundaries.

## Overview

The locales and text-break variants available for finding boundaries in Unicode text can be determined by calling the Locales Utilities functions `LocaleOperationCountLocales` and `LocaleOperationGetLocales` with the `opClass` parameter set to the `kUnicodeTextBreakClass` constant.

## Topics

### Constants

var kUnicodeTextBreakClass: Int

Identifies the class of Unicode utility operations that find text boundaries.

