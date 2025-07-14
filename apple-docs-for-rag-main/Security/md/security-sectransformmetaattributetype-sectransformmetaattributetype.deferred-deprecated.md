

- Security
- SecTransformMetaAttributeType
-  SecTransformMetaAttributeType.deferred Deprecated

Case

# SecTransformMetaAttributeType.deferred

The attribute defers notifications.

macOS 10.7–13.0Deprecated

``` source
case deferred
```

Deprecated

SecTransform is no longer supported

## Discussion

Determines if the AttributeSetNotification notification or the ProcessData blocks are deferred until SecTransformExecute(_:_:) is called. This metadata value has a default value of true for the input attribute but is false for all other attributes.

