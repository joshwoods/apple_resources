

- Objective-C Runtime
- NSObject
- NSObject.KeyValueObservingPublisher
-  object 

Instance Property

# object

The object that contains the property to publish.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
let object: Subject
```

## See Also

### Inspecting KVO Publisher Properties

let keyPath: KeyPath&lt;Subject, Value>

The key path, relative to the object receiving this message, of the property to publish.

let options: NSKeyValueObservingOptions

Options that determine which elements the publisher produces.

