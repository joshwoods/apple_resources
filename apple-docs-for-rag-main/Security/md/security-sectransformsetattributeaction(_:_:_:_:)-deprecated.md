

- Security
-  SecTransformSetAttributeAction(\_:\_:\_:\_:) Deprecated

Function

# SecTransformSetAttributeAction(\_:\_:\_:\_:)

Requests a callback when an attribute is set.

macOS 10.7–13.0Deprecated

``` source
func SecTransformSetAttributeAction(
    _ ref: SecTransformImplementationRef,
    _ action: CFString,
    _ attribute: SecTransformStringOrAttribute?,
    _ newAction: @escaping SecTransformAttributeActionBlock
) -> CFError?
```

Deprecated

SecTransform is no longer supported

## Parameters 

`ref`  

A SecTransformImplementationRef that is bound to an instance of a custom transform.

`action`  

The behavior to be set.

Use kSecTransformActionAttributeNotification to add a block that is called when an attribute is set. If the name is `NULL`, then the supplied block is called for all set attributes except for ones that have a specific block as a handler.

Use kSecTransformActionAttributeValidation to add a block that is called to validate the input to an attribute.

`attribute`  

The name of the attribute that will be handled. An attribute reference may also be given here. A `NULL` value indicates that the supplied action is for all attributes.

`newAction`  

A SecTransformAttributeActionBlock which implements the behavior.

## Return Value

An error on failure, or `NULL` on success. In Objective-C, call the CFRelease function to free the error’s memory when you are done with it.

## Discussion

The kSecTransformActionProcessData action used with the SecTransformSetDataAction(_:_:_:) function is a special case of a SecTransformSetAttributeAction(_:_:_:_:) action. If this is called on the input attribute then it will overwrite any kSecTransformActionProcessData action.

You may call this function multiple times for either a named attribute or for all attributes when the attribute parameter is `NULL`. The last call takes precedence.

