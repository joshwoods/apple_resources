

- Security
-  SecTransformFindByName(\_:\_:) Deprecated

Function

# SecTransformFindByName(\_:\_:)

Finds a member of a transform group by its name.

macOS 10.7–12.0Deprecated

``` source
func SecTransformFindByName(
    _ transform: SecGroupTransform,
    _ name: CFString
) -> SecTransform?
```

Deprecated

SecTransform is no longer supported

## Parameters 

`transform`  

The transform group to be searched.

`name`  

The name of the transform to be found.

## Return Value

The transform group member, or `NULL` if the member was not found.

## Discussion

When a transform instance is created you give it a unique name. This name can be used to find that instance in a group. While it is possible to use the SecTransformSetAttribute(_:_:_:_:) function to change a transform’s name after creating it, this is not recommended because doing so causes the SecTransformFindByName(_:_:) function to misbehave.

