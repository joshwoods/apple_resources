

- Application Services
- ColorSync Manager
-  NewCMFlattenUPP 

# NewCMFlattenUPP

Creates a new universal procedure pointer (UPP) to a data-flattening callback.

``` source
func NewCMFlattenUPP(_ userRoutine: CMFlattenProcPtr) -> CMFlattenUPP
```

## Parameters 

`userRoutine`  

A pointer to your data-flattening callback function.

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

