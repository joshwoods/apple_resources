

- Security
-  SecTransformActionBlock Deprecated

Type Alias

# SecTransformActionBlock

A block that overrides the default behavior of a custom transform.

macOS 10.7–13.0Deprecated

``` source
typealias SecTransformActionBlock = () -> Unmanaged?
```

Deprecated

SecTransform is no longer supported

## Return Value

A dictionary of the custom items to be exported if this block is used to override the kSecTransformActionExternalizeExtraData action or `NULL` for any other action. Alternatively, the block returns a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 object if an error occurs.

## Discussion

A block of this type is used to override the default behavior of a custom transform. This block is associated with the SecTransformOverrideTransformAction block.

The behaviors that can be overridden are:

- kSecTransformActionCanExecute - Determine if the transform has all of the data needed to run.

- kSecTransformActionStartingExecution - Called just before running ProcessData.

- kSecTransformActionFinalize - Called just before deleting the custom transform.

- kSecTransformActionExternalizeExtraData - Called to allow for writing out custom data to be exported.

For example:

```
SecTransformImplementationRef ref;
CFErrorRef error = NULL;

error = SecTransformSetTransformAction(ref, kSecTransformActionStartingExecution, ^{
    // Initialize any data needed before running
    CFErrorRef result = DoMyInitialization();
    return result;});

SecTransformTransformActionBlock actionBlock =
^{
    // Clean up any existing data before running
    CFErrorRef result = DoMyFinalization();
    return result;};

error = SecTransformSetTransformAction(ref, kSecTransformActionFinalize,actionBlock);
```

