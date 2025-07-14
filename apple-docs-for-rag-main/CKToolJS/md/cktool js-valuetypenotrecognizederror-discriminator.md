

- CKTool JS
- ValueTypeNotRecognizedError
-  discriminator 

Instance Property

# discriminator

The object’s type identifier.

CKTool JS 1.2.15+

``` source
attribute string discriminator;
```

## Discussion

For an object that’s part of a hierarchy, an object deserializer uses a discriminator value to determine what the JSON should be deserialized as. The deserializer function emits this error if the discriminator is unrecognized.

