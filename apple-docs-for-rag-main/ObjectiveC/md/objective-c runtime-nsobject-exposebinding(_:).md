

- Objective-C Runtime
- NSObject
-  exposeBinding(\_:) 

Type Method

# exposeBinding(\_:)

Exposes the specified `binding`, advertising its availability.

macOS

``` source
class func exposeBinding(_ binding: NSBindingName)
```

## Parameters 

`binding`  

The key path for the property to be exposed.

## Discussion

The bound property will be accessed using key-value-coding compliant methods. This method is typically invoked in the class’s `initialize` implementation.

Bindings exposed using `exposeBinding` will be exposed automatically in exposedBindings unless that method explicitly filters them out, for example in subclasses.

## See Also

### Exposing bindings

var exposedBindings: [NSBindingName]

Returns an array containing the bindings exposed by the receiver.

