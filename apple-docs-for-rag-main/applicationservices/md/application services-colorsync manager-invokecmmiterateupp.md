

- Application Services
- ColorSync Manager
-  InvokeCMMIterateUPP 

# InvokeCMMIterateUPP

Invokes a universal procedure pointer (UPP) to a progress-monitoring callback for the CMIterateCMMInfo function.

``` source
func InvokeCMMIterateUPP(_ iterateData: UnsafeMutablePointer, _ refCon: UnsafeMutablePointer, _ userUPP: CMMIterateUPP) -> OSErr
```

## Overview

In most cases, you do not need to call this function as ColorSync Manager invokes your callback for you. See the CMMIterateProcPtr callback for more information and for a description of the parameters.

## See Also

### Working With Universal Procedure Pointers

NewCMBitmapCallBackUPP

Creates a new universal procedure pointer (UPP) to a bitmap callback.

DisposeCMBitmapCallBackUPP

Disposes of a universal procedure pointer (UPP) to a bitmap callback.

InvokeCMBitmapCallBackUPP

Invokes a universal procedure pointer (UPP) to a bitmap callback.

NewCMConcatCallBackUPP

Creates a new universal procedure pointer (UPP) to a progress-monitoring callback.

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

NewCMProfileIterateUPP

Creates a new universal procedure pointer (UPP) to a profile-iteration callback.

DisposeCMProfileIterateUPP

Disposes of a universal procedure pointer (UPP) to a profile-iteration callback.

InvokeCMProfileIterateUPP

Invokes a universal procedure pointer (UPP) to a profile-iteration callback.

