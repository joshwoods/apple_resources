

- Security
- SecTransformMetaAttributeType
-  SecTransformMetaAttributeType.canCycle Deprecated

Case

# SecTransformMetaAttributeType.canCycle

The transform allows cyclic behavior.

macOS 10.7–13.0Deprecated

``` source
case canCycle
```

Deprecated

SecTransform is no longer supported

## Discussion

A transform group is a directed graph which is typically acyclic. Some transforms need to work with cycles. For example, a transform that emits a header and trailer around the data of another transform must create a cycle. If this metadata set to true, no error is returned if a cycle is detected for this attribute.

