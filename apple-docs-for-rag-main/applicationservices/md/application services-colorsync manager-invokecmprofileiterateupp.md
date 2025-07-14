

- Application Services
- ColorSync Manager
-  InvokeCMProfileIterateUPP 

# InvokeCMProfileIterateUPP

Invokes a universal procedure pointer (UPP) to a profile-iteration callback.

``` source
func InvokeCMProfileIterateUPP(_ iterateData: UnsafeMutablePointer, _ refCon: UnsafeMutablePointer, _ userUPP: CMProfileIterateUPP) -> OSErr
```

## Return Value

A result code. See Result Codes.

## Overview

In most cases, you do not need to call this function as ColorSync Manager invokes your callback for you. See the CMProfileIterateProcPtr callback for more information and for a description of the parameters.

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

InvokeCMMIterateUPP

Invokes a universal procedure pointer (UPP) to a progress-monitoring callback for the CMIterateCMMInfo function.

NewCMProfileIterateUPP

Creates a new universal procedure pointer (UPP) to a profile-iteration callback.

DisposeCMProfileIterateUPP

Disposes of a universal procedure pointer (UPP) to a profile-iteration callback.

