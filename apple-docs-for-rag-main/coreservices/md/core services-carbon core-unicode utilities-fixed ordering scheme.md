

- Core Services
- Carbon Core
- Unicode Utilities
-  Fixed Ordering Scheme 

# Fixed Ordering Scheme

Specifies to use the fixed ordering scheme.

## Overview

`UCCollateOptions` is a 32-bit value. Bits 0-23 are described in UCCollateOptions. The field consisting of bits 24-31 is used for values that specify which fixed ordering scheme to use with the function UCCompareTextNoLocale(_:_:_:_:_:_:_:). Currently only one such scheme is provided.

Constants are provided for setting and testing the `UCCollateOptions` field that specifies the ordering scheme. These values are described in Fixed Ordering Masks 1 and Fixed Ordering Masks 2.

## Topics

### Constants

var kUCCollateTypeHFSExtended: Int

