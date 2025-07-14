

- Objective-C Runtime
- NSObject
- NSObject.KeyValueObservingPublisher
-  init(object:keyPath:options:) 

Initializer

# init(object:keyPath:options:)

Creates a key-value observing publisher for the given combination of object and key path, using publishing behavior options you provide.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
init(
    object: Subject,
    keyPath: KeyPath,
    options: NSKeyValueObservingOptions
)
```

## Parameters 

`object`  

The object that contains the property to publish.

`keyPath`  

The key path, relative to the object receiving this message, of the property to publish.

`options`  

Options that determine which elements the publisher produces. Set this parameter to `[]` to receive new elements when the observed property changes.

## Discussion

This publisher produces a new element every time the observed property changes.

