

- Security
-  SecTransformSetDataAction(\_:\_:\_:) Deprecated

Function

# SecTransformSetDataAction(\_:\_:\_:)

Changes the way a custom transform processes data.

macOS 10.7–13.0Deprecated

``` source
func SecTransformSetDataAction(
    _ ref: SecTransformImplementationRef,
    _ action: CFString,
    _ newAction: @escaping SecTransformDataBlock
) -> CFError?
```

Deprecated

SecTransform is no longer supported

## Parameters 

`ref`  

A SecTransformImplementationRef that is bound to an instance of a custom transform.

`action`  

The action being overridden.

Use kSecTransformActionProcessData to change the way that input data is processed into the output data. The default behavior is to simply copy the input data to the output attribute. Changing this behavior is really a special case of a SecTransformSetAttributeAction(_:_:_:_:) action. Using kSecTransformActionProcessData as the `action` overwrites any previously set kSecTransformActionAttributeNotification action.

Use kSecTransformActionInternalizeExtraData to change the way that custom externalized data is imported into the transform. The default behavior is to do nothing.

`newAction`  

A SecTransformDataBlock which implements the behavior.

If the `action` parameter is kSecTransformActionProcessData then this block is called to process the input data into the output data. If the action parameter is kSecTransformActionInternalizeExtraData then this block is called to input custom data into the transform.

## Return Value

An error on failure, or `NULL` on success. In Objective-C, call the CFRelease function to free the error’s memory when you are done with it.

## Discussion

When the `action` parameter is kSecTransformActionProcessData, the `newAction` block changes the way that input data is processed to become the output data. When the `action` parameter is kSecTransformActionInternalizeExtraData it changes the way a custom transform reads in data to be imported into the transform.

You may call this function multiple times. The last call takes precedence.

