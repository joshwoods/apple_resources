

- Security
- SecTransformMetaAttributeType
-  SecTransformMetaAttributeType.ref Deprecated

Case

# SecTransformMetaAttributeType.ref

A direct reference to an attribute’s value.

macOS 10.7–13.0Deprecated

``` source
case ref
```

Deprecated

SecTransform is no longer supported

## Discussion

This reference allows for direct access to an attribute without having to look up the attribute by name. If a transform commonly uses an attribute, using a reference speeds up the use of that attribute. Attribute references are not visible or valid from outside of the particular transform instance.

