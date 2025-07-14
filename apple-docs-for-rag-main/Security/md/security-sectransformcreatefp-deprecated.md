

- Security
-  SecTransformCreateFP Deprecated

Type Alias

# SecTransformCreateFP

A pointer to a function that creates a new instance of a custom transform.

macOS 10.7–13.0Deprecated

``` source
typealias SecTransformCreateFP = (CFString, SecTransform, SecTransformImplementationRef) -> () -> Unmanaged?
```

Deprecated

SecTransform is no longer supported

## Parameters 

`name`  

The name of the new custom transform. This name must be unique.

`newTransform`  

The newly created transform.

`ref`  

A reference that is bound to an instance of a custom transform.

## Return Value

A SecTransformInstanceBlock that is used to create a new instance of a custom transform.

## Discussion

Provide a function of this type to the SecTransformCreate(_:_:) function when creating a custom transform. The function defined here returns an object of type SecTransformInstanceBlock that provides the implementation of all of the overrides necessary to create the custom transform. This returned SecTransformInstanceBlock is also where the “instance” variables for the custom transform may be defined.

