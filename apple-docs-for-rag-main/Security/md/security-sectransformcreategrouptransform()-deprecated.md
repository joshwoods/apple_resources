

- Security
-  SecTransformCreateGroupTransform() Deprecated

Function

# SecTransformCreateGroupTransform()

Creates an object that acts as a container for a set of connected transforms.

macOS 10.7–12.0Deprecated

``` source
func SecTransformCreateGroupTransform() -> SecGroupTransform
```

Deprecated

SecTransform is no longer supported

## Return Value

A transform group object.

## Discussion

A SecGroupTransform is a container for all of the transforms that are in a directed graph. You can use this container as you would a single transform with the SecTransformExecute(_:_:), SecTransformExecuteAsync(_:_:_:) and SecTransformCopyExternalRepresentation(_:) functions.On the other hand, unlike a stand alone transform, you can’t use a transform group with the SecTransformConnectTransforms(_:_:_:_:_:_:), SecTransformSetAttribute(_:_:_:_:) or SecTransformGetAttribute(_:_:) functions. Attempting to do so produces undefined behavior.

