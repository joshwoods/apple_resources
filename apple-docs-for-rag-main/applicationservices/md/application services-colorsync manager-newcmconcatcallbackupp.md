

- Application Services
- ColorSync Manager
-  NewCMConcatCallBackUPP 

# NewCMConcatCallBackUPP

Creates a new universal procedure pointer (UPP) to a progress-monitoring callback.

``` source
func NewCMConcatCallBackUPP(_ userRoutine: CMConcatCallBackProcPtr) -> CMConcatCallBackUPP
```

## Parameters 

`userRoutine`  

A pointer to your progress-monitoring callback function.

## Return Value

The universal procedure pointer.

## Overview

The callback protects against the appearance of a stalled machine during lengthy color world processing. If a CMM takes more than several seconds to process the information and create a color world, it will call the callback, if one is provided, and pass it the `refCon` provided. Passed to the functions `NCWNewLinkProfile` or `NCWConcatColorWorld` function .

## See Also

### Working With Universal Procedure Pointers

NewCMBitmapCallBackUPP

Creates a new universal procedure pointer (UPP) to a bitmap callback.

DisposeCMBitmapCallBackUPP

Disposes of a universal procedure pointer (UPP) to a bitmap callback.

InvokeCMBitmapCallBackUPP

Invokes a universal procedure pointer (UPP) to a bitmap callback.

DisposeCMConcatCallBackUPP

Disposes of a universal procedure pointer (UPP) to a progress-monitoring callback.

InvokeCMConcatCallBackUPP

Invokes a universal procedure pointer (UPP) to a progress-monitoring callback.

NewCMFlattenUPP

Creates a new universal procedure pointer (UPP) to a data-flattening callback.

DisposeCMFlattenUPP

Disposes of a universal procedure pointer (UPP) to a data-flattening callback.

InvokeCMFlattenUPP

Invokes a universal procedure pointer (UPP) to a data-flattening callback.

NewCMMIterateUPP

Creates a new universal procedure pointer (UPP) to a progress-monitoring callback for the `CMIterateCMMInfo` function.

DisposeCMMIterateUPP

Disposes of a universal procedure pointer (UPP) to a progress-monitoring callback for the `CMIterateCMMInfo` function.

InvokeCMMIterateUPP

Invokes a universal procedure pointer (UPP) to a progress-monitoring callback for the CMIterateCMMInfo function.

NewCMProfileIterateUPP

Creates a new universal procedure pointer (UPP) to a profile-iteration callback.

DisposeCMProfileIterateUPP

Disposes of a universal procedure pointer (UPP) to a profile-iteration callback.

InvokeCMProfileIterateUPP

Invokes a universal procedure pointer (UPP) to a profile-iteration callback.

