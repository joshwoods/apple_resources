

- Security
-  SecTransformSetTransformAction(\_:\_:\_:) Deprecated

Function

# SecTransformSetTransformAction(\_:\_:\_:)

Changes the way that a transform deals with transform lifecycle behaviors.

macOS 10.7–13.0Deprecated

``` source
func SecTransformSetTransformAction(
    _ ref: SecTransformImplementationRef,
    _ action: CFString,
    _ newAction: @escaping SecTransformActionBlock
) -> CFError?
```

Deprecated

SecTransform is no longer supported

## Parameters 

`ref`  

A custom transform.

`action`  

The behavior to change. Valid values are kSecTransformActionCanExecute, kSecTransformActionStartingExecution, kSecTransformActionFinalize, or kSecTransformActionExternalizeExtraData.

`newAction`  

A SecTransformActionBlock block that implements the behavior.

## Return Value

An error on failure, or `NULL` on success. In Objective-C, call the CFRelease function to free the error’s memory when you are done with it.

