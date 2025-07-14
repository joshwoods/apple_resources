

- Application Services
- ColorSync Manager
-  NewCMMIterateUPP 

# NewCMMIterateUPP

Creates a new universal procedure pointer (UPP) to a progress-monitoring callback for the `CMIterateCMMInfo` function.

``` source
func NewCMMIterateUPP(_ userRoutine: CMMIterateProcPtr) -> CMMIterateUPP
```

## Parameters 

`userRoutine`  

A pointer to your progress-monitoring callback function.

## Return Value

The universal procedure pointer.

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

