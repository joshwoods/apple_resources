

- Core Services
- Carbon Core
- Unicode Utilities
-  Fixed Ordering Masks 1 

# Fixed Ordering Masks 1

Set and test the `UCCollateOptions` field that specifies a fixed ordering scheme.

## Overview

You can use these constants to set or obtain a value that specifies a fixed ordering scheme. For a description of the available types of fixed ordering schemes, see Fixed Ordering Scheme.

For example, to specify `kUCCollateTypeHFSExtended` in the `options` parameter of the function UCCompareTextNoLocale(_:_:_:_:_:_:_:) , the `kUCCollateTypeHFSExtended` value must be shifted by `kUCCollateTypeShiftBits ` :

`options = kUCCollateTypeHFSExtended kUCCollateTypeShiftBits; `

You would obtain the ordering scheme value from the `options` parameter as follows:

fixedOrderType = ((options > > kUCCollateTypeShiftBits) &amp;  kUCCollateTypeSourceMask);

See also Fixed Ordering Masks 2.

## Topics

### Constants

var kUCCollateTypeSourceMask: Int

You can use this mask, in conjunction with the `kUCCollateTypeShiftBits` constant, to obtain a value identifying a fixed ordering scheme.

var kUCCollateTypeShiftBits: Int

