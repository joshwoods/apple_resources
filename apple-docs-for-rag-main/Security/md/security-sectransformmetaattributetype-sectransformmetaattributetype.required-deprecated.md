

- Security
- SecTransformMetaAttributeType
-  SecTransformMetaAttributeType.required Deprecated

Case

# SecTransformMetaAttributeType.required

Indicates whether the attribute value is optional.

macOS 10.7–13.0Deprecated

``` source
case required
```

Deprecated

SecTransform is no longer supported

## Discussion

Specifies if an attribute must have a non `NULL` value set or have an incoming connection before the transform starts to execute. This metadata has a default value of true for the input attribute, but false for all other attributes.

